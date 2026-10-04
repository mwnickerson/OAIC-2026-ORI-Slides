# ORI model card

Model: `gpt-6-luna-nous`; MCP pairing: `steven_external`.

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
| mcp | 49/50 | 50 | 50 | 52 | partial/diagnostic |
| mcp | 50/50 | 50 | 50 | 50 | partial/diagnostic |
| mcp | 48/50 | 50 | 48 | 50 | partial/diagnostic |
| mcp | 19/50 | 23 | 19 | 23 | partial/diagnostic |
| mcp | 48/50 | 50 | 49 | 50 | partial/diagnostic |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `openai/gpt-6-luna`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 1 | failed | 49/50 | 50/50 | 1,000,954 | 55,692 | not recorded | not recorded | not computed | none recorded |
| seed67-step1-six-models-3rep-3mcp-20260930 | 1 | failed | 50/50 | 50/50 | 955,622 | 53,920 | not recorded | not recorded | not computed | none recorded |
| seed67-step1-six-models-3rep-3mcp-20260930 | 2 | failed | 48/50 | 50/50 | 1,042,358 | 54,367 | not recorded | not recorded | not computed | INFRA_ERROR=1, OUTPUT_INVALID=1 |
| seed67-step1-six-models-3rep-3mcp-20260930 | 3 | failed | 19/50 | 23/50 | 393,957 | 28,419 | not recorded | not recorded | not computed | INFRA_ERROR=3, MISSING=27, OUTPUT_INVALID=1 |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | 1 | failed | 48/50 | 50/50 | 1,096,087 | 50,704 | not recorded | not recorded | not computed | OUTPUT_INVALID=1 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/0/results/12`, `analysis.json#/analyses/1/results/9`, `analysis.json#/analyses/1/results/10`, `analysis.json#/analyses/1/results/11`, `analysis.json#/analyses/3/results/3`.
