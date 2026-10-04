# ORI model card

Model: `qwen3.8-flash-nous`; MCP pairing: `armadin`.

Source integrity: structural checks of ORI public report projection only; no cryptographic attestation.
Benchmark completion: partial/incomplete.
Analysis coverage: public aggregate report and question-level summaries only; private evidence was not opened.
Publication status: not published.
Diagnostic artifact unless all source validations and comparison gates pass.
Direct and MCP tracks are not combined. MCP differences are not causal evidence.
Scores below are ORI-reported facts; incomplete slots remain in scheduled denominators.

## Results

| Track | Correct / scheduled | Attempted | Graded | Attempts | Status |
|---|---:|---:|---:|---:|---|
| mcp | 12/50 | 50 | 38 | 60 | partial/diagnostic |
| mcp | 14/50 | 50 | 37 | 59 | partial/diagnostic |
| mcp | 0/50 | 1 | 0 | 1 | partial/diagnostic |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `qwen/qwen3.8-flash`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 1 | failed | 12/50 | 50/50 | 16,752,225 | 299,148 | not recorded | not recorded | not computed | INFRA_ERROR=6, OUTPUT_INVALID=6 |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 2 | failed | 14/50 | 50/50 | 16,081,333 | 260,831 | not recorded | not recorded | not computed | INFRA_ERROR=9, OUTPUT_INVALID=4 |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 3 | failed | 0/50 | 1/50 | 58,620 | 3,618 | not recorded | not recorded | not computed | INFRA_ERROR=1, MISSING=49 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/0/results/6`, `analysis.json#/analyses/0/results/7`, `analysis.json#/analyses/0/results/8`.

### Operator-supplied Armadin/HTTP-400 finding
The operator reports 34 HTTP 400 responses after successful MCP tool-call turns: 26 associated with tasks ending in `INFRA_ERROR`, and 8 in records that ultimately completed. The position-9 example followed an `analyze_group_permissions` result of 3,710,830 characters, with a reconstructed follow-up request estimated at 4.49 MB. Smaller failures and larger successes mean payload size is a possible contributor, not a proven threshold. The response body was not saved; the exact rejection reason is unknown. The operator says the harness used broad `PROVIDER_PROTOCOL` classification. These are infrastructure/protocol outcomes, not reasoning errors. See the executive summary for repetition-3 coverage and the separate Steven External teardown note. Private task attempts were not reopened.
