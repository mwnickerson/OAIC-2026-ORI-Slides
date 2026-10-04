# ORI model card

Model: `qwen3.8-27b-q4km`; MCP pairing: `none`.

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
| direct | 6/50 | 50 | 6 | 50 | partial/diagnostic |
| direct | 6/50 | 21 | 7 | 21 | partial/diagnostic |
| direct | 0/50 | 0 | 0 | 0 | partial/diagnostic |
| direct | 29/50 | 50 | 31 | 50 | completed |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `qwen3.8-27b-q4km-262k`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | interrupted | 6/50 | 50/50 | 5,781 | 3,469 | not recorded | not recorded | not computed | TASK_TIMEOUT=44 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | interrupted | 6/50 | 21/50 | 5,938 | 3,994 | not recorded | not recorded | not computed | INTERRUPTED=1, MISSING=29, TASK_TIMEOUT=13 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | interrupted | 0/50 | 0/50 | 0 | 0 | not recorded | not recorded | not computed | MISSING=50 |
| qwen3.8-json-rerun-2 | 1 | completed | 29/50 | 50/50 | 72,877 | 240,112 | not recorded | not recorded | not computed | OUTPUT_INVALID=17, QUERY_ERROR=2 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/1/results/36`, `analysis.json#/analyses/1/results/37`, `analysis.json#/analyses/1/results/38`, `analysis.json#/analyses/6/results/0`.
