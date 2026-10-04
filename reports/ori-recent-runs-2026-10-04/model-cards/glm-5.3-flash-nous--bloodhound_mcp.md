# ORI model card

Model: `glm-5.3-flash-nous`; MCP pairing: `bloodhound_mcp`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `z-ai/glm-5.3-flash`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| glm53flash-shared-matrix-seed67-3mcp-20260929 | 1 | 28 | 16 | 44 | 50 | 6 | OUTPUT_INVALID=6 | OUTPUT_INVALID=6 | 3,560,397 | 215,239 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/4/results/1` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 23 | 17 | 40 | 50 | 10 | OUTPUT_INVALID=10 | OUTPUT_INVALID=10 | 3,873,158 | 238,233 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/15` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 26 | 12 | 38 | 50 | 12 | OUTPUT_INVALID=12 | OUTPUT_INVALID=12 | 3,420,612 | 206,900 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/16` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 24 | 13 | 37 | 50 | 13 | OUTPUT_INVALID=13 | OUTPUT_INVALID=13 | 3,580,255 | 215,812 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/17` |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | 1 | 26 | 17 | 43 | 50 | 7 | OUTPUT_INVALID=7 | OUTPUT_INVALID=7 | 4,658,343 | 239,209 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/5/results/1` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
