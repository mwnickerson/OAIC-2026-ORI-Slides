# ORI model card

Model: `qwen3.8-flash-nous`; MCP pairing: `none`.

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
| direct | 31/50 | 50 | 34 | 50 | completed |
| direct | 35/50 | 50 | 37 | 50 | completed |
| direct | 30/50 | 50 | 34 | 50 | completed |
| direct | 31/50 | 50 | 33 | 50 | completed |

## Methods and limitations

Source is ORI's public aggregate report. Task records and attempt transcripts were not read. Source integrity is structural only; lifecycle/evidence verification is bounded to the public projection. See analysis.json for row-cited findings.


## Usage, cost, and operational notes

Provider(s): `openai-compat`. Exact provider-model ID(s): `qwen/qwen3.8-flash`.
Input/output values are provider-reported aggregate counters. Cache-token categories and API charges are not in the public projections. “Not recorded” is not zero spend; no rate estimate is made without dated exact-model rates and cache/input/output breakdown.

| Run/cohort | Rep | State | Correct/scheduled | Attempted/scheduled | Input tokens | Output tokens | Cache tokens | Recorded cost | Estimate | Failure tallies |
|---|---:|---|---:|---:|---:|---:|---|---:|---:|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 1 | completed | 31/50 | 50/50 | 72,877 | 223,753 | not recorded | not recorded | not computed | OUTPUT_INVALID=13, QUERY_ERROR=3 |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 2 | completed | 35/50 | 50/50 | 72,877 | 222,265 | not recorded | not recorded | not computed | OUTPUT_INVALID=12, QUERY_ERROR=1 |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | 3 | completed | 30/50 | 50/50 | 72,877 | 223,611 | not recorded | not recorded | not computed | OUTPUT_INVALID=12, QUERY_ERROR=4 |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | 1 | completed | 31/50 | 50/50 | 72,877 | 204,221 | not recorded | not recorded | not computed | OUTPUT_INVALID=11, QUERY_ERROR=6 |

Keep failed, missing, interrupted and in-flight slots in the scheduled denominator. Tallies are public aggregates and may include retries/events, not necessarily unique tasks. A completed row can still contain output-format or query errors.
Source pointers: `analysis.json#/analyses/0/results/0`, `analysis.json#/analyses/0/results/1`, `analysis.json#/analyses/0/results/2`, `analysis.json#/analyses/5/results/2`.
