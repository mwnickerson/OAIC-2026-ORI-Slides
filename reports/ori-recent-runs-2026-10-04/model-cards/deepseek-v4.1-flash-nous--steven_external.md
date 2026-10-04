# ORI model card

Model: `deepseek-v4.1-flash-nous`; MCP pairing: `steven_external`.

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
| mcp | 35/50 | 50 | 47 | 50 | partial/diagnostic |
| mcp | 35/50 | 50 | 47 | 50 | partial/diagnostic |
| mcp | 34/50 | 50 | 47 | 50 | partial/diagnostic |
| mcp | 36/50 | 50 | 47 | 50 | partial/diagnostic |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `deepseek/deepseek-v4.1-flash`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | failed | 35/50 | 50/50 | 3,543,294 | 112,405 | not recorded | not recorded | not computed | OUTPUT_INVALID=3 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | failed | 35/50 | 50/50 | 3,214,823 | 111,013 | not recorded | not recorded | not computed | OUTPUT_INVALID=3 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | failed | 34/50 | 50/50 | 3,601,558 | 117,168 | not recorded | not recorded | not computed | OUTPUT_INVALID=3 |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | 1 | failed | 36/50 | 50/50 | 3,199,701 | 115,412 | not recorded | not recorded | not computed | OUTPUT_INVALID=3 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/1/results/33`, `analysis.json#/analyses/1/results/34`, `analysis.json#/analyses/1/results/35`, `analysis.json#/analyses/2/results/3`.
