# ORI model card

Model: `gemma-4-26b-it-qat-q4-0-64k`; MCP pairing: `bloodhound_mcp`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `gemma-4-26b-it-qat-q4_0-64k`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | 0 | 0 | not recorded | not recorded | not computed | Missing/interrupted · unscored | `analysis.json#/analyses/1/results/63` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | 0 | 0 | not recorded | not recorded | not computed | Missing/interrupted · unscored | `analysis.json#/analyses/1/results/64` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | 0 | 0 | not recorded | not recorded | not computed | Missing/interrupted · unscored | `analysis.json#/analyses/1/results/65` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
