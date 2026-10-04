# ORI model card

Model: `qwen3.8-flash-nous`; MCP pairing: `armadin`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `qwen/qwen3.8-flash`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 1 | 12 | 26 | 38 | 50 | 12 | INFRA_ERROR=6, OUTPUT_INVALID=6 | INFRA_ERROR=6, OUTPUT_INVALID=6 | 16,752,225 | 299,148 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/0/results/6` |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 2 | 14 | 23 | 37 | 50 | 13 | INFRA_ERROR=9, OUTPUT_INVALID=4 | INFRA_ERROR=9, OUTPUT_INVALID=4 | 16,081,333 | 260,831 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/0/results/7` |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 3 | 0 | 0 | 0 | 50 | 50 | INFRA_ERROR=1, MISSING=49 | INFRA_ERROR=1, MISSING=49 | 58,620 | 3,618 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/0/results/8` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
