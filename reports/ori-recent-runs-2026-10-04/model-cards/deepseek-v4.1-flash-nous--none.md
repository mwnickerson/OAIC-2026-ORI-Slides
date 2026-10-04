# ORI model card

Model: `deepseek-v4.1-flash-nous`; MCP pairing: `none`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `deepseek/deepseek-v4.1-flash`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | 1 | 29 | 4 | 33 | 50 | 17 | QUERY_ERROR=4, QUERY_TIMEOUT=1, TASK_TIMEOUT=12 | QUERY_ERROR=4, QUERY_TIMEOUT=1, TASK_TIMEOUT=12 | 55,337 | 108,431 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/2/results/0` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 32 | 5 | 37 | 50 | 13 | OUTPUT_INVALID=3, QUERY_ERROR=5, TASK_TIMEOUT=5 | OUTPUT_INVALID=3, QUERY_ERROR=5, TASK_TIMEOUT=5 | 67,660 | 122,262 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/1/results/24` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 35 | 3 | 38 | 50 | 12 | OUTPUT_INVALID=7, QUERY_ERROR=5 | OUTPUT_INVALID=7, QUERY_ERROR=5 | 75,667 | 160,100 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/25` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 32 | 3 | 35 | 50 | 15 | OUTPUT_INVALID=10, QUERY_ERROR=5 | OUTPUT_INVALID=10, QUERY_ERROR=5 | 75,788 | 187,569 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/26` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
