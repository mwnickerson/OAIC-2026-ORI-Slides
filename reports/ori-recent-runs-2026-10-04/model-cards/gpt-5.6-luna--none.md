# ORI model card

Model: `gpt-5.6-luna`; MCP pairing: `none`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `codex`. Provider model ID(s): `gpt-5.6-luna`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | 1 | 0 | 0 | 0 | 50 | 50 | INFRA_ERROR=3, MISSING=47 | INFRA_ERROR=3, MISSING=47 | 0 | 0 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/5/results/6` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
