# ORI model card

Model: `glm-5.3-flash-nous`; MCP pairing: `steven_external`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `z-ai/glm-5.3-flash`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| glm53flash-shared-matrix-seed67-3mcp-20260929 | 1 | 31 | 16 | 47 | 50 | 3 | OUTPUT_INVALID=3 | OUTPUT_INVALID=3 | 2,793,762 | 165,375 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/4/results/3` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 27 | 18 | 45 | 50 | 5 | INFRA_ERROR=1, OUTPUT_INVALID=4 | INFRA_ERROR=1, OUTPUT_INVALID=4 | 3,604,580 | 182,699 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/21` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 30 | 15 | 45 | 50 | 5 | INFRA_ERROR=1, OUTPUT_INVALID=4 | INFRA_ERROR=1, OUTPUT_INVALID=4 | 3,784,174 | 168,821 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/22` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 30 | 13 | 43 | 50 | 7 | OUTPUT_INVALID=7 | OUTPUT_INVALID=7 | 8,506,073 | 158,462 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/23` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
