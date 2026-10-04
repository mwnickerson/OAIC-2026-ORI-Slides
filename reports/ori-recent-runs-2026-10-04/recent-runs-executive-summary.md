# ORI · All Recent Report-Ready Runs

**Scope:** the seven public-report roots modified Sept 28–Oct 3, 2026: three campaigns under `results/benchmark-runs` plus the latest four direct-child report directories. Older Sept 27-and-earlier direct-child reports are outside this pass. Every included root had an ORI `report.json`.

## Headline

- 7 report roots; 114 aggregate result rows; 10 model labels; 5,700 scheduled slots and 3,635 attempted. The report-root summaries are partial; result-slot states vary.
- State counts: completed=32, failed=46, interrupted=3, unknown=33. These are lifecycle labels, not an accuracy score.
- All 21 cross-root pairs failed ORI’s compatibility gate. No single cross-run leaderboard or pooled accuracy is presented.
- Direct and MCP are separate. Repetitions remain repetitions, not extra independent questions.
- The separate GLM-5.3 Flash shared-matrix run is included, as is GLM’s three-repetition slice inside the six-model campaign.

## Included report roots

| Report root | Status | Result rows | Scheduled | Attempted | Model labels |
|---|---|---:|---:|---:|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | partial | 13 | 650 | 601 | gpt-6-luna-nous, qwen3.8-flash-nous |
| seed67-step1-six-models-3rep-3mcp-20260930 | partial | 72 | 3600 | 1844 | deepseek-v4.1-flash-nous, gemma-4-26b-it-qat-q4-0-64k, glm-5.3-flash-nous, gpt-6-luna-nous, muse-glimmer-30b, qwen3.8-27b-q4km |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | partial | 4 | 200 | 200 | deepseek-v4.1-flash-nous |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | partial | 8 | 400 | 373 | gpt-5.6-luna-nous, gpt-6-luna-nous |
| glm53flash-shared-matrix-seed67-3mcp-20260929 | partial | 4 | 200 | 200 | glm-5.3-flash-nous |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | partial | 8 | 400 | 212 | glm-5.3-flash-nous, gpt-5.6-luna, gpt-6-luna, qwen3.8-flash-nous |
| qwen3.8-json-rerun-2 | partial | 5 | 250 | 205 | qwen3.8-27b-q4km |

## Recent infrastructure incident: Qwen3.8 Flash / Armadin

The recovery report’s public aggregate rows are shown below. The detailed HTTP-400 interpretation is operator-supplied; private task-attempt files were not reopened.

| Report root | Rep | Correct/scheduled | Attempted/scheduled | State | Public failure tallies |
|---|---:|---:|---:|---|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 1 | 12/50 | 50/50 | failed | INFRA_ERROR=6, OUTPUT_INVALID=6 |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 2 | 14/50 | 50/50 | failed | INFRA_ERROR=9, OUTPUT_INVALID=4 |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 3 | 0/50 | 1/50 | failed | INFRA_ERROR=1, MISSING=49 |

Operator-supplied finding: the Armadin runs received 34 HTTP 400s after successful MCP tool-call turns; 26 were associated with final `INFRA_ERROR` tasks and 8 with records that ultimately completed. In repetition 3 there were 49 unexecuted questions. A repeated position-9 failure followed an `analyze_group_permissions` result of 3,710,830 characters, with a reconstructed follow-up request estimated at 4.49 MB.

Caveat: payload size may have contributed, but no single size threshold is established—smaller requests also failed and larger requests succeeded. The HTTP response body was not saved, so the exact rejection reason is unknown. The operator says the harness used broad `PROVIDER_PROTOCOL` classification. Keep these as infrastructure/protocol outcomes in the scheduled denominator, not reasoning errors. Steven External cleanup errors are separate teardown issues.

## Public aggregate outcome tallies

Tallies across selected report roots (aggregate events/retries, not necessarily unique tasks): `INFRA_ERROR`=73, `INTERRUPTED`=1, `MISSING`=2065, `OUTPUT_INVALID`=324, `QUERY_ERROR`=66, `QUERY_TIMEOUT`=13, `TASK_TIMEOUT`=76. Infrastructure failures, timeouts, invalid output, and missing work remain in the scheduled denominator.

## API usage and cost

Input/output token counters are present in 114/114 public result rows. Recorded-cost fields (`cost_usd`, `recorded_cost_usd`) are present in 0/114. Cache-token categories available: none in these public aggregates.
No Nous Portal billed usage export, cache breakdown, or dated rate snapshot is included. Cost is therefore marked **not recorded / not computed**, not zero. No dollar estimate is invented from token totals. Each Markdown card lists provider/model ID, per-repetition input/output tokens, and cost/cache availability.

## Comparison and evidence limits

ORI rejected every one of the 21 cross-root pairs because the task contract was unavailable/different and/or track/repetition scheduled cohorts differed. Matching seed 67 and question-set fingerprint alone do not establish compatibility.
All seven sources are public `report.json` projections. Structural public-projection validation is not cryptographic attestation. The attempt-level HTTP 400 story above is attributed to the operator, not independently verified. No credentials, `.env`, sealed answers, private traces, or task-attempt JSONs were opened.

## Files

- `analysis.md` / `analysis.html` / `analysis.pdf` / `analysis.json` — standard ORI analyzer output for the seven explicitly selected roots.
- `model-cards/` — 37 model/MCP-pairing cards; Markdown includes repetitions, token usage, cost availability, errors, and caveats; PNGs carry a cost/cache-not-recorded footer.
- `recent-runs-executive-summary.html` / `.pdf` — readable overview with all 114 public aggregate result rows.
- `recent-runs-bundle.zip` — complete deliverable.
- ORI-default visual style is used pending your S/C template choice.
