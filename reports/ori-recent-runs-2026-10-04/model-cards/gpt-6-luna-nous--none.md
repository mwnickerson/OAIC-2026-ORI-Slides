# ORI model card

Model: `gpt-6-luna-nous`; MCP pairing: `none`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `openai/gpt-6-luna`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| luna-nous-shared-matrix-seed67-3mcp-20260929 | 1 | 46 | 1 | 47 | 50 | 3 | QUERY_ERROR=1, QUERY_TIMEOUT=2 | QUERY_ERROR=1, QUERY_TIMEOUT=2 | 69,514 | 29,572 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/3/results/0` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 40 | 1 | 41 | 50 | 9 | QUERY_ERROR=3, QUERY_TIMEOUT=6 | QUERY_ERROR=3, QUERY_TIMEOUT=6 | 69,514 | 27,603 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/1/results/0` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 43 | 2 | 45 | 50 | 5 | QUERY_ERROR=4, QUERY_TIMEOUT=1 | QUERY_ERROR=4, QUERY_TIMEOUT=1 | 69,514 | 27,166 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/1/results/1` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 45 | 0 | 45 | 50 | 5 | QUERY_ERROR=3, QUERY_TIMEOUT=2 | QUERY_ERROR=3, QUERY_TIMEOUT=2 | 69,514 | 25,151 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/1/results/2` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
