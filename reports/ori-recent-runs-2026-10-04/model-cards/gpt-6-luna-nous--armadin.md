# ORI model card

Model: `gpt-6-luna-nous`; MCP pairing: `armadin`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `openai/gpt-6-luna`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| luna-nous-shared-matrix-seed67-3mcp-20260929 | 1 | 30 | 19 | 49 | 50 | 1 | INFRA_ERROR=1 | INFRA_ERROR=1 | 7,462,100 | 66,904 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/3/results/2` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 32 | 16 | 48 | 50 | 2 | INFRA_ERROR=1, OUTPUT_INVALID=1 | INFRA_ERROR=1, OUTPUT_INVALID=1 | 6,939,957 | 65,526 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/6` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 32 | 15 | 47 | 50 | 3 | INFRA_ERROR=2, OUTPUT_INVALID=1 | INFRA_ERROR=2, OUTPUT_INVALID=1 | 7,325,529 | 61,717 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/7` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 31 | 16 | 47 | 50 | 3 | INFRA_ERROR=2, OUTPUT_INVALID=1 | INFRA_ERROR=2, OUTPUT_INVALID=1 | 8,102,137 | 61,169 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/8` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
