# ORI: speaker talking points

A condensed outline of Matthew Nickerson's OAIC 2026 talk, in slide order.

[Slides (PDF)](slides/ori-oaic-2026.pdf) · [Recent-run reports and model cards](reports/ori-recent-runs-2026-10-04/)

## 01 — [Stop Giving Models Open-Book Tests](slides/ori-oaic-2026.pdf#page=1)

- I wanted to know whether a model could inspect an unfamiliar Active Directory graph and work out a useful attack path, rather than repeat a familiar lab walkthrough.
- That became the Offensive Reasoning Index: synthetic BloodHound data and questions, evaluated through Direct Cypher or MCP tools.
- Getting useful results meant fixing the data, questions, and grader. Finding a graph path does not prove a model can run a red-team engagement.

## 02 — [A model worth using](slides/ori-oaic-2026.pdf#page=2)

- I'm Matthew Nickerson. I work in adversary simulation at SpecterOps, and I'm a local-LLM enthusiast.
- I'd already worked on a BloodHound MCP. I wanted a reasonably small model to do useful BloodHound work, and I wanted to know where it would fall over.
- My first questions came from things I could answer myself. I ran the Cypher through the API and checked it in the GUI.
- If I couldn't explain the expected answer, that was a bad place to start testing somebody else's reasoning.

## 03 — [My MCP needed a fair test](slides/ori-oaic-2026.pdf#page=3)

- I'd seen an external comparison using GOAD and wanted a grounded way to compare my own MCP and improve it.
- GOAD was context, not ORI's starting dataset. I worried about familiarity; I don't have evidence that a particular model memorized it.
- A result mixes the model, tools, graph, and question. I needed to hold the test still for comparisons and change the environment deliberately.

## 04 — [Same seed. Same test.](slides/ori-oaic-2026.pdf#page=4)

- Seed 67 has no special meaning. It starts repeatable pseudorandom choices for the generated environment—not the model's own randomness. Pin the generator version, profile, and settings as well as the seed.
- Identity and size use separate seeded streams. The identity stream is `seeded-benchmark-v1:complex:67:identity`; it chooses a fictional company and domain from fixed lists. The complex base ranges are 4,500–5,500 users, 1,750–2,250 workstations, and 400–600 servers. Templates can add entities beyond these base counts.
- Seeded names and graph choices fill roles in prescribed attack-path templates. Departments and built-in groups follow fixed rules, so changing the seed need not change every element.
- The generator writes a ZIP and manifest. Task questions compile separately using entities from that environment; the seed does not select question templates. Current scope stays seed 67 only. [Mechanics and audit limits](references/data/ref-12-seed-mechanics.md).

## 05 — [Before reasoning, the data had to load](slides/ori-oaic-2026.pdf#page=5)

- BloodHound initially couldn't read what I generated: missing fields, wrong edges, wrong node labels. I was fixing JSON before learning much about the model.
- My rough progress indicator was upload versus ingestion failure. Failed to upload meant very bad; failed to ingest meant I was getting closer.
- Fixes included `functionallevel`, `GPOChanges`, and how I represented `AdminTo`. An edge in my generator wasn't enough; the imported graph was what mattered.

## 06 — [The first win was a very small question](slides/ori-oaic-2026.pdf#page=6)

- My first proof of concept used a small model on my RTX 3080. I don't remember which model. After struggling with ingestion, seeing it work surprised me.
- An early example, reconstructed from verification notes, asked which user had an active session on a particular workstation.
- That's small enough to check by hand. If the relationship never reached BloodHound, a more elaborate prompt won't put it back.

## 07 — [A random seed does not stop the clock](slides/ori-oaic-2026.pdf#page=7)

- A later repeatability problem was literal: the clock was still running. Seeded offsets repeated, but their wall-clock base changed.
- Normalizing fields such as `pwdlastset` and `lastlogon` addressed data timestamps. ZIP entry timestamps needed separate handling.
- Identical parsed JSON doesn't guarantee an identical archive. I want to know that a changed score didn't come from quietly changing the test data.

## 08 — [From graph to grade](slides/ori-oaic-2026.pdf#page=8)

- Generate the graph and tasks, import into BloodHound, give the model its public question, execute its query or tool loop, then grade and save the result.
- The model gets the acceptance rules, not the private reference answer.
- The documented early Direct harness executed reference and model Cypher, then compared results using task rules. It didn't just ask whether the query looked like mine. Contract versions belong with results.

## 09 — [Two routes to the same graph](slides/ori-oaic-2026.pdf#page=9)

- Direct asks the model for a Cypher query; the harness executes it and evaluates the result.
- MCP gives the model a tool loop: request a tool, receive an observation, decide what comes next, and submit an answer.
- Both depend on BloodHound evidence. One Direct query can traverse a long path. Shared questions don't mean identical interfaces or scoring contracts.

## 10 — [The prompt is part of the experiment](slides/ori-oaic-2026.pdf#page=10)

- Historical Direct instructions required only a Cypher query, without explanation or markdown. That was a bare-query contract.
- The current ordinary runner uses JSON. MCP requires one object matching `submission_schema` and says, "Do not invent graph evidence." Direct uses JSON containing a bounded read-only query and declared assertions.
- Changing the answer shape or what the parser accepts changes the experiment, even when the graph question sounds the same.

## 11 — [My grader missed correct answers](slides/ori-oaic-2026.pdf#page=11)

- My earliest scorer was barebones. Exact matching missed some correct answers, so I had to improve it before trusting the score.
- The documented Phase 2 grader executed queries and compared results. Different query text can produce the right evidence.
- Later, identity aliases mattered too: an object ID and display name can name the same entity. Normalization should recognize correct work, not replace a wrong entity with the one I wanted.

## 12 — [From local GPUs to hosted models](slides/ori-oaic-2026.pdf#page=12)

- I started with an M4 Mac, a 3080, and a 3090. I still want a useful smallish model, especially with an MCP.
- Codex-login support expanded access to OpenAI models; thanks to Adam Chester for that implementation. OpenAI-compatible providers added routes such as NOUS Portal and OpenRouter.
- The ORI runner and model inference can live in different places. A report saved on my GPU rig doesn't prove the weights ran there.

## 13 — [When the easy questions stopped helping](slides/ori-oaic-2026.pdf#page=13)

- With frontier models available, earlier questions were often too easy to tell me what I wanted to know. Many needed one correct query.
- One query is not one graph hop. I wanted intermediate steps the model had to investigate and connect.
- Tasks progressed toward combined techniques, longer chains, misleading alternatives, and nonviable routes. More nodes alone aren't the interesting part; the permissions have to connect into a useful path.

## 14 — [From finding a path to explaining it](slides/ori-oaic-2026.pdf#page=14)

- An early saved question asked for a full attack path between a user and a domain controller. The recovered trace had a Cypher error; it wasn't a successful answer.
- The later Tier 6 template asks for multiple lookups, the host/user/group sequence, each hop's mechanism, and the terminal Tier 0 condition.
- It also asks the model to reject attractive dead ends. I want to inspect how the intermediate steps connect.

## 15 — [Four hosts to Domain Admins](slides/ori-oaic-2026.pdf#page=15)

- This generator template has four hosts and nine relationships: an initial `CanPSRemote` foothold, followed by session discoveries and administrative pivots.
- `HasSession` goes from computer to user; `AdminTo` goes from principal to computer. The model must preserve which identity gains the next access, ending at Domain Admins membership.
- The code's three-host name counts three administrative pivots after the foothold. The actual chain uses four machines and has no decoy branch.

## 16 — [Same path. Real graph.](slides/ori-oaic-2026.pdf#page=16)

- This is the same session-pivot chain imported into BloodHound from ORI's seed-67 dataset.
- Starting with SWEAVER, `CanPSRemote` reaches the first host. Sessions and the next identity's `AdminTo` access lead to MBRADLEY and Domain Admins membership.
- The relationship directions matter; the model can't invent a shortcut. This demonstrates the imported graph, not that a model solved the task.

## 17 — [A tool call in name only](slides/ori-oaic-2026.pdf#page=17)

- Qwen2.5-Coder 14B led an early Direct cohort but failed in the MCP workflow by emitting pseudo-tool-call JSON.
- Printing a tool name and arguments isn't issuing a call, receiving a result, and using it. I need the interaction record to tell the difference.
- Provider failure, invalid output, and never submitting a final answer need different fixes from a wrong path. One bad score hides those distinctions.

## 18 — [The answer was there. Parsing hid it.](slides/ori-oaic-2026.pdf#page=18)

- The September 26 BloodHound MCP audit started with a recorded 3/50 correct.
- An offline diagnostic extracted existing JSON from surrounding prose and fences. With answer facts unchanged, the saved outputs yielded 34/50.
- There were no new model calls or repaired entities. This was a diagnostic replay, not a replacement official score.
- A later fresh Qwen run also scored 34/50. That matching number is coincidence, not the same evidence.

## 19 — [Beyond the score](slides/ori-oaic-2026.pdf#page=19)

- Right plus wrong equals scored; scored plus unscored equals scheduled. Attempted requests are a different count. An infrastructure error, invalid output, query error, timeout, or missing evaluation is not automatically a scored wrong answer.
- Keep final unscored-question causes separate from historical retries, tool-error events, campaign lifecycle, and teardown notes. Cleanup can fail after usable answers have already been scored.
- Alongside outcomes, ORI retains model prompts/answers and provider-exposed reasoning, queries, tool and resource activity, reported usage/timing, and run identities. Availability is provider-dependent; exposed reasoning is not access to hidden internal reasoning.
- The corrected [question ledger](reports/ori-recent-runs-2026-10-04/question-scoring-ledger.json) and [status ledger](reports/ori-recent-runs-2026-10-04/presentation-status-ledger.json) explain the coverage counts.

## 20 — [Benchmarks on a budget](slides/ori-oaic-2026.pdf#page=20)

- I wanted runs to finish in roughly one to two hours without becoming extremely expensive, not a guarantee for every campaign.
- I focused on smaller, Flash, and affordable models, generally targeting paid APIs below $5 per million output tokens. That's a selection target, not measured task cost.
- Anthropic API costs were prohibitive for my budget. This isn't a strongest-model leaderboard.
- September 28 and the newer matrix requested 8,192 output tokens per response, 600 seconds per Direct task, and 1,200 per MCP task. Other settings differ; an MCP task can contain multiple responses.

## 21 — [One run isn't the whole story](slides/ori-oaic-2026.pdf#page=21)

- I am sticking with seed 67 for the current benchmark, not adding a three-seed run. The three passes repeat the same 50 questions on the same generated graph.
- We have three-pass results and a separate recovery campaign, but the full six-model campaign was interrupted. Coverage stays beside scores.
- Repeated passes do not establish generalization across environments, and a fixed data seed does not guarantee identical model sampling.

## 22 — [ORI in action](slides/ori-oaic-2026.pdf#page=22)

- My planned demonstration follows configuration, generation, ingestion, benchmarking, and inspection, using one model and one MCP to keep the workflow clear.
- The generated ZIP and reference manifest must match the dataset loaded into BloodHound. A healthy connection doesn't establish graph identity.
- I want to connect an actual submitted answer with its verdict, distinguishing wrong evidence from formatting problems, tool failures, and unfinished work.
- ORI produces the scores. Hermes can explain saved results in a report, but I check its numbers and examples against the artifacts. A confident paragraph doesn't get to change the denominator.

## 23 — [Early local scorecards](slides/ori-oaic-2026.pdf#page=23)

- These are separate historical campaigns, not a leaderboard or measured improvement across a fixed test.
- Phase 3A Direct recorded 3/20 for Qwen2.5-Coder 14B and 2/20 for Qwen3; Cypher errors mattered.
- Phase 3B tools-only recorded 21/40 for Qwen3.5 9B and 18/40 for Qwen3 14B.
- The May 3 resources run recorded 28/40 for Gemma4-26B at 64k. Phase 4 full MCP recorded 22/43 for Gemma e4b at 64k and 20/43 for Qwen3.5 9B. Models, tasks, and interfaces changed.

## 24 — [Different tests, separate scorecards](slides/ori-oaic-2026.pdf#page=24)

- Complex V1 recorded 44/62 for GPT-5.6 Sol and 46/62 for GPT-5.5. Known grading defects make these development history, not a ranking.
- V29 Direct used five passes of 42 fixed tasks: 210 scheduled evaluations per model. GPT-5.5, Daybreak Red, Daybreak Blue, and GPT-5.6 Sol scored 207, 206, 205, and 204.
- Their observed ranges overlap and aren't confidence intervals. Small differences don't establish durable ordering; neither panel belongs in an average with current shared-question runs.

## 25 — [Three passes, final scores](slides/ori-oaic-2026.pdf#page=25)

- The final benchmark repeats the same 50 seed-67 questions three times: 150 scheduled evaluations per model–route pairing, not 150 distinct questions or three environments.
- In Direct / BloodHound MCP / Armadin / Steven order, correct totals are GPT-6 Luna 128 / 145 / 95 / 147; GLM 113 / 73 / 51 / 87; DeepSeek 99 / 82 / 73 / 104; Qwen Flash 96 / 82 / 26 / 70.
- GPT-6 Luna with Steven has 147 right, one wrong, 148 scored and two unscored, with all 150 attempted. Correct counts per pass are 50, 48 and 49.
- Qwen Flash with Armadin attempted 101 of 150 and scored 75: 26 right, 49 wrong and 75 unscored. Its coverage gap belongs to that row only.
- The model–tool pairing matters. This is one fixed question set, and Direct and MCP use different scoring contracts; it is not a universal ranking. Keep per-pass results and unscored coverage visible.
- [Final benchmark selection and exact score/token tables](references/data/ref-13-final-benchmark.md).

## 26 — [Where the tokens went](slides/ori-oaic-2026.pdf#page=26)

- Token usage covers the same selected final three-pass benchmark. The table reports exact input, output and total tokens for every model–route pairing, plus input share.
- GPT-6 Luna with Steven used 2,998,934 input and 163,979 output tokens: 3,162,913 total, 94.8% input. GPT-6 Luna with Armadin used 22,367,623 input and 188,412 output: 22,556,035 total, 99.2% input.
- The selected-run totals include recorded retry attempts and exclude the superseded whole repetition. They are not whole-project spending.
- Qwen Flash with Armadin has 101/150 attempted coverage, so its raw token total is not a like-for-like full-run cost comparison. All other displayed pairings attempted 150/150.
- MCP can accumulate tool schemas, returned data and previous turns in repeated requests. Provider-reported token volume is not a verified dollar bill; billing and cache breakdowns are missing.
- [Final benchmark selection and exact score/token tables](references/data/ref-13-final-benchmark.md).

## 27 — [When the API rejects the request](slides/ori-oaic-2026.pdf#page=27)

- One saved analyze_group_permissions response contained 3,710,830 characters/UTF-8 bytes. That tool output becomes part of the conversation sent back to the model.
- Saved messages plus 97 tool schemas reconstruct to 4,486,453–4,486,502 compact UTF-8 bytes, about 4.49 MB. This is a reconstructed request core, not captured HTTP wire bytes or a measured token count.
- HTTP 400 rejections were observed, but the provider rejection body was not saved. The exact cause and size/context limit remain unknown; size is not established as the cause.
- This is a request-design observation, not a deduction from the final scores. Keep useful tool evidence without returning an entire world of data for every step.
- [Sanitized request-size evidence](references/data/ref-09-request-size.json).

## 28 — [The next questions for ORI](slides/ori-oaic-2026.pdf#page=28)

- I want to generate Azure BloodHound data and test reasoning over its cloud identity attack paths.
- Then I'd like OpenGraph data, starting with collectors such as GitHound and JamfHound.
- I'm interested in model-as-judge approaches, possibly Jev or an open-source alternative, checked against known answers before relying on them.
- I'd also like to test Fable, Astra, and Kimi when budget permits. These are research ideas and next steps, not finished capabilities or results.

## 29 — [The score is a starting point](slides/ori-oaic-2026.pdf#page=29)

- I want people to run models they care about: small or large, local or hosted, through MCP or Direct Cypher.
- Learn the setup's shortcomings before treating a plausible answer as reliable. ORI tests bounded graph reasoning, not general offensive capability.
- The questions need to stay useful, and the harness needs scrutiny. Some failures belonged to my benchmark. Keep configuration and failures with the score, then improve the model, agent, or tools.

## 30 — [Your next benchmark](slides/ori-oaic-2026.pdf#page=30)

- ORI's repository is `offensive-reasoning-index` under SpecterOps on GitHub.
- Run the models and tool setups you care about.
- Inspect where they fall short.

## 31 — [Acknowledgements](slides/ori-oaic-2026.pdf#page=31)

- Competition drives innovation. Without other people's BloodHound MCP work, I probably wouldn't have come up with ORI.
- I'm especially thankful to Brett from Armadin for his blog post and for answering my questions about their MCP and evaluation approach.
- Thank you to the Armadin team, Steven, and MorDavid for their MCPs.
- Thanks to SpecterOps for BloodHound and internal testing, especially Blaise; and to Kyle from Outflank for contributions to my BloodHound MCP.

## 32 — [References](slides/ori-oaic-2026.pdf#page=32)

- Unspoken appendix. [13](references/data/ref-13-final-benchmark.md) supplies the final three-pass selection, scores, coverage and exact token totals; [12](references/data/ref-12-seed-mechanics.md) explains generation and the seed. [Earlier references](references/README.md) retain their historical or diagnostic meanings.
