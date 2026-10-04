# ORI model card

Model: `gpt-6-luna-nous`; MCP pairing: `bloodhound_mcp`.

Source integrity: structural validation of public ORI report projections; not cryptographic attestation.
Benchmark completion: parent report root status is listed per source in `question-scoring-ledger.json`; individual rows below use scoring coverage/cause labels.
Analysis coverage: public aggregate and public question-result rows only. Private attempts were not opened.
Publication status: not published.

Direct and MCP results remain separate. Repetitions remain separate observations; no pooled score or causal MCP claim is made.

Provider(s): `openai-compat`. Provider model ID(s): `openai/gpt-6-luna`.
Counts: right + wrong = scored; unscored = scheduled − scored. Public question outcomes explain unscored rows where available. Attempt/error tallies are shown separately because retries/events need not equal unique questions.

| Run | Rep | Right | Wrong | Scored | Scheduled | Unscored | Unscored outcome causes | Attempt/error tallies | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Presentation status | Source |
|---|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---:|---:|---|---|
| luna-nous-shared-matrix-seed67-3mcp-20260929 | 1 | 49 | 1 | 50 | 50 | 0 | none reported | none reported | 2,076,245 | 71,777 | not recorded | not recorded | not computed | All scheduled scored | `analysis.json#/analyses/3/results/1` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | 47 | 2 | 49 | 50 | 1 | INFRA_ERROR=1 | INFRA_ERROR=1 | 6,759,534 | 63,188 | not recorded | not recorded | not computed | Provider/infra issue · unscored | `analysis.json#/analyses/1/results/3` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | 49 | 0 | 49 | 50 | 1 | OUTPUT_INVALID=1 | OUTPUT_INVALID=1 | 1,729,339 | 69,862 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/4` |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | 49 | 0 | 49 | 50 | 1 | OUTPUT_INVALID=1 | OUTPUT_INVALID=1 | 1,825,229 | 64,001 | not recorded | not recorded | not computed | Output-validation issue · unscored | `analysis.json#/analyses/1/results/5` |

API cost and cache status: token input/output counters are shown above; `cost_usd` and `recorded_cost_usd` are null across the selected public rows, cache-token categories and dated Nous Portal rate data are absent. Cost is unavailable, not zero; no estimate is invented.
Infrastructure interpretation: provider/infra, timeout, output-validation, missing, interruption, and teardown labels describe public outcome evidence; they are not labels of reasoning capability. See the executive report for the operator-supplied Qwen Flash/Armadin incident note.
