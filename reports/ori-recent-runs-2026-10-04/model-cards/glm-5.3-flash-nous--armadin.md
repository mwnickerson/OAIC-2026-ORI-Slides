# ORI model card

Model: `glm-5.3-flash-nous`; MCP pairing: `armadin`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `z-ai/glm-5.3-flash`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| glm53flash-shared-matrix-seed67-3mcp-20260929 | 1 | 16 | 26 | 42 | 50 | 8 | INFRA_ERROR=2, OUTPUT_INVALID=6 | INFRA_ERROR=2, OUTPUT_INVALID=6 | 12,688,092 | 265,827 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/4/results/2` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 15 | 24 | 39 | 50 | 11 | INFRA_ERROR=2, OUTPUT_INVALID=9 | INFRA_ERROR=2, OUTPUT_INVALID=9 | 11,053,249 | 237,281 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/18` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 19 | 22 | 41 | 50 | 9 | INFRA_ERROR=2, OUTPUT_INVALID=7 | INFRA_ERROR=2, OUTPUT_INVALID=7 | 12,339,853 | 261,255 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/19` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 17 | 20 | 37 | 50 | 13 | INFRA_ERROR=3, OUTPUT_INVALID=10 | INFRA_ERROR=3, OUTPUT_INVALID=10 | 10,473,220 | 238,148 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/20` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
