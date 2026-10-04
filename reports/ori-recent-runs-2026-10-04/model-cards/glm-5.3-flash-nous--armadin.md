# ORI model card

Model: `glm-5.3-flash-nous`; MCP pairing: `armadin`.

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
| mcp | 15/50 | 50 | 39 | 50 | partial/diagnostic |
| mcp | 19/50 | 50 | 41 | 50 | partial/diagnostic |
| mcp | 17/50 | 50 | 37 | 50 | partial/diagnostic |
| mcp | 16/50 | 50 | 42 | 50 | partial/diagnostic |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `z-ai/glm-5.3-flash`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | failed | 15/50 | 50/50 | 11,053,249 | 237,281 | not recorded | not recorded | not computed | INFRA_ERROR=2, OUTPUT_INVALID=9 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | failed | 19/50 | 50/50 | 12,339,853 | 261,255 | not recorded | not recorded | not computed | INFRA_ERROR=2, OUTPUT_INVALID=7 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | failed | 17/50 | 50/50 | 10,473,220 | 238,148 | not recorded | not recorded | not computed | INFRA_ERROR=3, OUTPUT_INVALID=10 |
| glm53flash-shared-matrix-seed67-3mcp-20260929 | 1 | failed | 16/50 | 50/50 | 12,688,092 | 265,827 | not recorded | not recorded | not computed | INFRA_ERROR=2, OUTPUT_INVALID=6 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/1/results/18`, `analysis.json#/analyses/1/results/19`, `analysis.json#/analyses/1/results/20`, `analysis.json#/analyses/4/results/2`.
