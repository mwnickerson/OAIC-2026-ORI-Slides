# ORI model card

Model: `deepseek-v4.1-flash-nous`; MCP pairing: `bloodhound_mcp`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `deepseek/deepseek-v4.1-flash`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | 1 | 38 | 7 | 45 | 50 | 5 | INFRA_ERROR=1, OUTPUT_INVALID=4 | INFRA_ERROR=1, OUTPUT_INVALID=4 | 3,702,436 | 145,245 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/2/results/1` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 28 | 18 | 46 | 50 | 4 | OUTPUT_INVALID=4 | OUTPUT_INVALID=4 | 3,717,946 | 143,970 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/27` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 27 | 20 | 47 | 50 | 3 | OUTPUT_INVALID=3 | OUTPUT_INVALID=3 | 4,638,146 | 133,760 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/28` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 27 | 19 | 46 | 50 | 4 | OUTPUT_INVALID=4 | OUTPUT_INVALID=4 | 4,579,378 | 137,714 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/29` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
