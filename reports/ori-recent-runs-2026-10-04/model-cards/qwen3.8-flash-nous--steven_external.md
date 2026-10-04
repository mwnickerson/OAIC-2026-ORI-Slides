# ORI model card

Model: `qwen3.8-flash-nous`; MCP pairing: `steven_external`.

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
| mcp | 21/50 | 50 | 45 | 51 | partial/diagnostic |
| mcp | 26/50 | 50 | 45 | 50 | partial/diagnostic |
| mcp | 23/50 | 50 | 44 | 50 | partial/diagnostic |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `qwen/qwen3.8-flash`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 1 | failed | 21/50 | 50/50 | 5,076,049 | 224,279 | not recorded | not recorded | not computed | OUTPUT_INVALID=5 |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 2 | failed | 26/50 | 50/50 | 5,078,756 | 229,593 | not recorded | not recorded | not computed | OUTPUT_INVALID=5 |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 3 | failed | 23/50 | 50/50 | 4,060,369 | 208,992 | not recorded | not recorded | not computed | OUTPUT_INVALID=6 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/0/results/9`, `analysis.json#/analyses/0/results/10`, `analysis.json#/analyses/0/results/11`.
