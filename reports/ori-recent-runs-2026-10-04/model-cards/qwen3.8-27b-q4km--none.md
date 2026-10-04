# ORI model card

Model: `qwen3.8-27b-q4km`; MCP pairing: `none`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `qwen3.8-27b-q4km-262k`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| qwen3.8-json-rerun-2 | 1 | 29 | 2 | 31 | 50 | 19 | OUTPUT_INVALID=17, QUERY_ERROR=2 | OUTPUT_INVALID=17, QUERY_ERROR=2 | 72,877 | 240,112 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/6/results/0` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 6 | 0 | 6 | 50 | 44 | TASK_TIMEOUT=44 | TASK_TIMEOUT=44 | 5,781 | 3,469 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/1/results/36` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 6 | 1 | 7 | 50 | 43 | INTERRUPTED=1, MISSING=29, TASK_TIMEOUT=13 | INTERRUPTED=1, MISSING=29, TASK_TIMEOUT=13 | 5,938 | 3,994 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/1/results/37` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | 0 | 0 | not recorded | not recorded | not computed | Missing/interrupted · unscored | `analysis.json#/analyses/1/results/38` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
