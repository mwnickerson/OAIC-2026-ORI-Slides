# ORI model card

Model: `glm-5.3-flash-nous`; MCP pairing: `none`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `z-ai/glm-5.3-flash`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| glm53flash-shared-matrix-seed67-3mcp-20260929 | 1 | 39 | 2 | 41 | 50 | 9 | OUTPUT_INVALID=7, QUERY_ERROR=2 | OUTPUT_INVALID=7, QUERY_ERROR=2 | 70,427 | 140,165 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/4/results/0` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 38 | 3 | 41 | 50 | 9 | OUTPUT_INVALID=5, QUERY_ERROR=4 | OUTPUT_INVALID=5, QUERY_ERROR=4 | 70,427 | 155,420 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/12` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 39 | 4 | 43 | 50 | 7 | OUTPUT_INVALID=5, QUERY_ERROR=2 | OUTPUT_INVALID=5, QUERY_ERROR=2 | 70,427 | 126,222 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/13` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 36 | 1 | 37 | 50 | 13 | OUTPUT_INVALID=9, QUERY_ERROR=4 | OUTPUT_INVALID=9, QUERY_ERROR=4 | 68,115 | 126,720 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/14` |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | 1 | 44 | 0 | 44 | 50 | 6 | OUTPUT_INVALID=2, QUERY_ERROR=3, QUERY_TIMEOUT=1 | OUTPUT_INVALID=2, QUERY_ERROR=3, QUERY_TIMEOUT=1 | 70,427 | 128,485 | not recorded | not recorded | not computed | Timeout-affected · unscored | `analysis.json#/analyses/5/results/0` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
