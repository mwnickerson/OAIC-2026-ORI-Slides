# ORI model card

Model: `glm-5.3-flash-nous`; MCP pairing: `none`.

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
| direct | 38/50 | 50 | 41 | 50 | completed |
| direct | 39/50 | 50 | 43 | 50 | completed |
| direct | 36/50 | 50 | 37 | 50 | completed |
| direct | 39/50 | 50 | 41 | 50 | completed |
| direct | 44/50 | 50 | 44 | 50 | completed |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `z-ai/glm-5.3-flash`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | completed | 38/50 | 50/50 | 70,427 | 155,420 | not recorded | not recorded | not computed | OUTPUT_INVALID=5, QUERY_ERROR=4 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | completed | 39/50 | 50/50 | 70,427 | 126,222 | not recorded | not recorded | not computed | OUTPUT_INVALID=5, QUERY_ERROR=2 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | completed | 36/50 | 50/50 | 68,115 | 126,720 | not recorded | not recorded | not computed | OUTPUT_INVALID=9, QUERY_ERROR=4 |
| glm53flash-shared-matrix-seed67-3mcp-20260929 | 1 | completed | 39/50 | 50/50 | 70,427 | 140,165 | not recorded | not recorded | not computed | OUTPUT_INVALID=7, QUERY_ERROR=2 |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | 1 | completed | 44/50 | 50/50 | 70,427 | 128,485 | not recorded | not recorded | not computed | OUTPUT_INVALID=2, QUERY_ERROR=3, QUERY_TIMEOUT=1 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/1/results/12`, `analysis.json#/analyses/1/results/13`, `analysis.json#/analyses/1/results/14`, `analysis.json#/analyses/4/results/0`, `analysis.json#/analyses/5/results/0`.
