# ORI model card

Model: `gpt-6-luna-nous`; MCP pairing: `none`.

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
| direct | 40/50 | 50 | 41 | 50 | completed |
| direct | 43/50 | 50 | 45 | 50 | completed |
| direct | 45/50 | 50 | 45 | 50 | completed |
| direct | 46/50 | 50 | 47 | 50 | completed |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `openai/gpt-6-luna`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | completed | 40/50 | 50/50 | 69,514 | 27,603 | not recorded | not recorded | not computed | QUERY_ERROR=3, QUERY_TIMEOUT=6 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | completed | 43/50 | 50/50 | 69,514 | 27,166 | not recorded | not recorded | not computed | QUERY_ERROR=4, QUERY_TIMEOUT=1 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | completed | 45/50 | 50/50 | 69,514 | 25,151 | not recorded | not recorded | not computed | QUERY_ERROR=3, QUERY_TIMEOUT=2 |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | 1 | completed | 46/50 | 50/50 | 69,514 | 29,572 | not recorded | not recorded | not computed | QUERY_ERROR=1, QUERY_TIMEOUT=2 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/1/results/0`, `analysis.json#/analyses/1/results/1`, `analysis.json#/analyses/1/results/2`, `analysis.json#/analyses/3/results/0`.
