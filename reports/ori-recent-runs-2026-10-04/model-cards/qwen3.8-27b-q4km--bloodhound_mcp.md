# ORI model card

Model: `qwen3.8-27b-q4km`; MCP pairing: `bloodhound_mcp`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `qwen3.8-27b-q4km-262k`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| qwen3.8-json-rerun-2 | 1 | 34 | 10 | 44 | 50 | 6 | INFRA_ERROR=2, OUTPUT_INVALID=4 | INFRA_ERROR=2, OUTPUT_INVALID=4 | 4,020,835 | 237,571 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/6/results/1` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | 0 | 0 | not recorded | not recorded | not computed | Missing/interrupted · unscored | `analysis.json#/analyses/1/results/39` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | 0 | 0 | not recorded | not recorded | not computed | Missing/interrupted · unscored | `analysis.json#/analyses/1/results/40` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | 0 | 0 | not recorded | not recorded | not computed | Missing/interrupted · unscored | `analysis.json#/analyses/1/results/41` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
