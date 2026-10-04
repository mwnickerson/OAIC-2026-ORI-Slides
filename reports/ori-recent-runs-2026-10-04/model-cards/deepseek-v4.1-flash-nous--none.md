# ORI model card

Model: `deepseek-v4.1-flash-nous`; MCP pairing: `none`.

Source integrity: structural checks of ORI public report projection only; no cryptographic attestation.
Benchmark completion: reported complete (not independently revalidated).
Analysis coverage: public aggregate report and question-level summaries only; private evidence was not opened.
Publication status: not published.
Diagnostic artifact unless all source validations and comparison gates pass.
Direct and MCP tracks are not combined. MCP differences are not causal evidence.
Scores below are ORI-reported facts; incomplete slots remain in scheduled denominators.

## Results

| Track | Correct / scheduled | Attempted | Graded | Attempts | Status |
|---|---:|---:|---:|---:|---|
| direct | 32/50 | 50 | 37 | 50 | completed |
| direct | 35/50 | 50 | 38 | 50 | completed |
| direct | 32/50 | 50 | 35 | 50 | completed |
| direct | 29/50 | 50 | 33 | 50 | completed |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `deepseek/deepseek-v4.1-flash`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | completed | 32/50 | 50/50 | 67,660 | 122,262 | not recorded | not recorded | not computed | OUTPUT_INVALID=3, QUERY_ERROR=5, TASK_TIMEOUT=5 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | completed | 35/50 | 50/50 | 75,667 | 160,100 | not recorded | not recorded | not computed | OUTPUT_INVALID=7, QUERY_ERROR=5 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | completed | 32/50 | 50/50 | 75,788 | 187,569 | not recorded | not recorded | not computed | OUTPUT_INVALID=10, QUERY_ERROR=5 |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | 1 | completed | 29/50 | 50/50 | 55,337 | 108,431 | not recorded | not recorded | not computed | QUERY_ERROR=4, QUERY_TIMEOUT=1, TASK_TIMEOUT=12 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/1/results/24`, `analysis.json#/analyses/1/results/25`, `analysis.json#/analyses/1/results/26`, `analysis.json#/analyses/2/results/0`.
