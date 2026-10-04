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

- Seed 67 controls graph generation and concrete questions for these conference runs. With code and configuration fixed, I can regenerate the test. I am keeping the current benchmark on seed 67.
- That does not make model inference deterministic or make familiar attack techniques unfamiliar. It changes the graph facts the model must inspect.
- I checked repeatability by generating repeatedly, diffing JSON, and inspecting paths in BloodHound. A matching seed is only the beginning of that check.

## 05 — [The first win was a very small question](slides/ori-oaic-2026.pdf#page=5)

- My first proof of concept used a small model on my RTX 3080. I don't remember which model. After struggling with ingestion, seeing it work surprised me.
- An early example, reconstructed from verification notes, asked which user had an active session on a particular workstation.
- That's small enough to check by hand. If the relationship never reached BloodHound, a more elaborate prompt won't put it back.

## 06 — [Before reasoning, the data had to load](slides/ori-oaic-2026.pdf#page=6)

- BloodHound initially couldn't read what I generated: missing fields, wrong edges, wrong node labels. I was fixing JSON before learning much about the model.
- My rough progress indicator was upload versus ingestion failure. Failed to upload meant very bad; failed to ingest meant I was getting closer.
- Fixes included `functionallevel`, `GPOChanges`, and how I represented `AdminTo`. An edge in my generator wasn't enough; the imported graph was what mattered.

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

- I want scheduled, attempted, graded, and correct counts beside failures and missing work. Wrong answers, invalid output, and timeouts need different fixes.
- Saved prompts, turns, queries, and answers help explain what happened. Provider-exposed reasoning text isn't access to hidden reasoning.
- Tool and resource records show requests and responses; a response doesn't prove successful execution or useful resource loading.
- Tokens, task time, and attempt history add context. Missing usage isn't free inference, and tokens aren't a dollar bill.
- The latest task outcome determines the score; recorded consumption includes earlier attempts. Model identity, seed, and fingerprints tie those records to their run.

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

## 25 — [The questions that never ran](slides/ori-oaic-2026.pdf#page=25)

- The local Qwen JSON rerun attempted 205/250 scheduled tasks. Correct counts were Direct 29/50, BloodHound 34/50, Mordavid 2/50, Armadin 20/50, and Steven 35/50.
- Every route except Mordavid attempted all 50. Mordavid attempted only five; three consecutive provider-protocol infrastructure failures triggered a cutoff, leaving 45 unexecuted. The full [five-route aggregate](references/data/ref-08-local-qwen.csv) retains the partial/cleanup labels.
- Steven attempted all 50: 35 correct, nine incorrect, five invalid outputs, and one infrastructure error. Cleanup failed afterward, so the route remained partial.
- The campaign failed and its report is partial. I need useful answers and a setup that reliably gets through the run.

## 26 — [Direct and MCP can disagree](slides/ori-oaic-2026.pdf#page=26)

- September 28 used NOUS-hosted GLM-5.3-Flash and Qwen-3.8-Flash, not the local Qwen setup.
- All four NOUS-hosted groups attempted 50 questions once. GLM scored Direct 44/50 versus BloodHound MCP 26/50; Qwen scored 31/50 versus 24/50.
- Direct used `direct-v2`; MCP used `mcp-answer-v1`. These observations don't establish a general MCP penalty. The larger campaign was partial, and infrastructure cutoffs elsewhere aren't a reasoning ranking.
- Four login-provider groups—GPT-6 Luna Direct, GPT-6 Luna BloodHound MCP, GPT-5.6 Luna Direct, and GPT-5.6 Luna BloodHound MCP—each stopped after 3/50 attempts: three infrastructure failures, zero graded answers, and 47 missing. That is not a measured zero reasoning score, and the report does not establish authentication as the cause.

## 27 — [The model–MCP matchup](slides/ori-oaic-2026.pdf#page=27)

- In Direct/BloodHound/Armadin/Steven order, single-pass scores were GLM 39/28/16/31, GPT-6 Luna 46/49/30/48, DeepSeek 29/38/23/36, and GPT-5.6 Luna 42/18/35/44. Every denominator is 50 scheduled.
- DeepSeek attempted all tasks, but its MCP groups were partial; Direct had 12 task timeouts.
- GPT-5.6 BloodHound attempted only 23 tasks through 26 attempts, leaving 27 unexecuted. Its 18/50 isn't a completed reasoning test.
- The campaigns failed with partial reports. Sampling and scoring contracts differ. I need to test a model with its specific MCP, not assume MCP always helps.

## 28 — [Where the tokens went](slides/ori-oaic-2026.pdf#page=28)

- This usage comparison returns to September 28, not the newer matrix. BloodHound MCP recorded about 4.90 million tokens for GLM and 6.24 million for Qwen.
- Input accounted for 95.1% and 95.4%. Corresponding Direct totals were much smaller.
- The groups recorded 423 and 504 tool requests, with four and ten failed responses. Those are events, not incorrect-task counts.
- That input volume deserves investigation, but it doesn't prove waste or establish a dollar price.

## 29 — [Three passes, same questions](slides/ori-oaic-2026.pdf#page=29)

- This campaign repeated 50 seed-67 questions three times: 150 scheduled evaluations per cell, not 150 unique questions.
- GPT-6 Luna with BloodHound MCP scored 47, 49, and 49, totaling 145/150. That's encouraging on this fixed test, not proof of generalization.
- The campaign was interrupted. Local Qwen partly ran; Muse and Gemma weren't reached. GPT's Steven route attempted 123/150. Those missing evaluations stay in view; recovery is separate.

## 30 — [Recovery is a separate result](slides/ori-oaic-2026.pdf#page=30)

- Recovery used cloud Qwen3.8 Flash, not the interrupted campaign's local Qwen. Scores were Direct 96/150, BloodHound 82/150, Armadin 26/150, and Steven 70/150.
- Armadin attempted 101/150, leaving 49 unexecuted. That isn't a completed reasoning test.
- GPT-6 Luna with Steven separately scored 49/50 in one recovery repetition, but cleanup failed. Its settings fingerprint differs, so I haven't spliced it into the original three-pass total.

## 31 — [An API rejection isn't a wrong answer](slides/ori-oaic-2026.pdf#page=31)

- The original campaign recorded 18 latest HTTP 400 outcomes: 16 on Armadin and two on Steven.
- Recovery still had 16 latest HTTP 400 outcomes on Qwen with Armadin, plus 49 unexecuted evaluations after an infrastructure cutoff. Its 34 historical failed attempts split into 26 on records ultimately ending in infrastructure error and eight on records that ultimately completed; those are attempts, not distinct failed questions.
- The [bounded size audit](references/data/ref-09-request-size.json) verified a 3,710,830-character `analyze_group_permissions` result. Saved messages plus 97 tool schemas reconstruct to about 4.49 MB of core JSON—not captured full-request or wire bytes.
- I suspect oversized requests or accumulated context. The retained error is only Bad Request; the provider's rejection body and size limit weren't saved, so that cause isn't confirmed.
- These are infrastructure failures and coverage gaps, not wrong reasoning. Recovery doesn't establish a fix.

## 32 — [The next questions for ORI](slides/ori-oaic-2026.pdf#page=32)

- I want to generate Azure BloodHound data and test reasoning over its cloud identity attack paths.
- Then I'd like OpenGraph data, starting with collectors such as GitHound and JamfHound.
- I'm interested in model-as-judge approaches, possibly Jev or an open-source alternative, checked against known answers before relying on them.
- I'd also like to test Fable, Astra, and Kimi when budget permits. These are research ideas and next steps, not finished capabilities or results.

## 33 — [The score is a starting point](slides/ori-oaic-2026.pdf#page=33)

- I want people to run models they care about: small or large, local or hosted, through MCP or Direct Cypher.
- Learn the setup's shortcomings before treating a plausible answer as reliable. ORI tests bounded graph reasoning, not general offensive capability.
- The questions need to stay useful, and the harness needs scrutiny. Some failures belonged to my benchmark. Keep configuration and failures with the score, then improve the model, agent, or tools.

## 34 — [Your next benchmark](slides/ori-oaic-2026.pdf#page=34)

- ORI's repository is `offensive-reasoning-index` under SpecterOps on GitHub.
- Run the models and tool setups you care about.
- Inspect where they fall short.

## 35 — [Acknowledgements](slides/ori-oaic-2026.pdf#page=35)

- Competition drives innovation. Without other people's BloodHound MCP work, I probably wouldn't have come up with ORI.
- I'm especially thankful to Brett from Armadin for his blog post and for answering my questions about their MCP and evaluation approach.
- Thank you to the Armadin team, Steven, and MorDavid for their MCPs.
- Thanks to SpecterOps for BloodHound and internal testing, especially Blaise; and to Kyle from Outflank for contributions to my BloodHound MCP.

## 36 — [References](slides/ori-oaic-2026.pdf#page=36)

Unspoken appendix. The slide lists the talk's references; the [recent-run reports and model cards](reports/ori-recent-runs-2026-10-04/) provide the accompanying results and qualifications.
