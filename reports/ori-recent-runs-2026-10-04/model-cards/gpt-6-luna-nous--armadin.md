# ORI model card

Model: `gpt-6-luna-nous`; MCP pairing: `armadin`.

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
| mcp | 32/50 | 50 | 48 | 50 | partial/diagnostic |
| mcp | 32/50 | 50 | 47 | 50 | partial/diagnostic |
| mcp | 31/50 | 50 | 47 | 50 | partial/diagnostic |
| mcp | 30/50 | 50 | 49 | 51 | partial/diagnostic |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `openai/gpt-6-luna`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | failed | 32/50 | 50/50 | 6,939,957 | 65,526 | not recorded | not recorded | not computed | INFRA_ERROR=1, OUTPUT_INVALID=1 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | failed | 32/50 | 50/50 | 7,325,529 | 61,717 | not recorded | not recorded | not computed | INFRA_ERROR=2, OUTPUT_INVALID=1 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | failed | 31/50 | 50/50 | 8,102,137 | 61,169 | not recorded | not recorded | not computed | INFRA_ERROR=2, OUTPUT_INVALID=1 |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | 1 | failed | 30/50 | 50/50 | 7,462,100 | 66,904 | not recorded | not recorded | not computed | INFRA_ERROR=1 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/1/results/6`, `analysis.json#/analyses/1/results/7`, `analysis.json#/analyses/1/results/8`, `analysis.json#/analyses/3/results/2`.
