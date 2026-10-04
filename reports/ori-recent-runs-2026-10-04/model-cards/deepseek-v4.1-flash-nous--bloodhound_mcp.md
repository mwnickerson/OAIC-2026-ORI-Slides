# ORI model card

Model: `deepseek-v4.1-flash-nous`; MCP pairing: `bloodhound_mcp`.

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
| mcp | 28/50 | 50 | 46 | 50 | completed |
| mcp | 27/50 | 50 | 47 | 50 | completed |
| mcp | 27/50 | 50 | 46 | 50 | completed |
| mcp | 38/50 | 50 | 45 | 50 | partial/diagnostic |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `deepseek/deepseek-v4.1-flash`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | completed | 28/50 | 50/50 | 3,717,946 | 143,970 | not recorded | not recorded | not computed | OUTPUT_INVALID=4 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | completed | 27/50 | 50/50 | 4,638,146 | 133,760 | not recorded | not recorded | not computed | OUTPUT_INVALID=3 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | completed | 27/50 | 50/50 | 4,579,378 | 137,714 | not recorded | not recorded | not computed | OUTPUT_INVALID=4 |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | 1 | failed | 38/50 | 50/50 | 3,702,436 | 145,245 | not recorded | not recorded | not computed | INFRA_ERROR=1, OUTPUT_INVALID=4 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/1/results/27`, `analysis.json#/analyses/1/results/28`, `analysis.json#/analyses/1/results/29`, `analysis.json#/analyses/2/results/1`.
