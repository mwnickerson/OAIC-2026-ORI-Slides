# ORI model card

Model: `qwen3.8-flash-nous`; MCP pairing: `bloodhound_mcp`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `qwen/qwen3.8-flash`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 1 | 28 | 17 | 45 | 50 | 5 | OUTPUT_INVALID=5 | OUTPUT_INVALID=5 | 5,190,803 | 269,754 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/0/results/3` |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 2 | 26 | 18 | 44 | 50 | 6 | OUTPUT_INVALID=6 | OUTPUT_INVALID=6 | 8,921,784 | 270,805 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/0/results/4` |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 3 | 28 | 17 | 45 | 50 | 5 | OUTPUT_INVALID=5 | OUTPUT_INVALID=5 | 5,799,142 | 243,653 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/0/results/5` |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | 1 | 24 | 20 | 44 | 50 | 6 | OUTPUT_INVALID=6 | OUTPUT_INVALID=6 | 5,954,035 | 285,032 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/5/results/3` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
