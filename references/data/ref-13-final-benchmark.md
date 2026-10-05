# Final three-run benchmark and token usage

This is the final presentation selection for seed 67: four hosted models, Direct plus three MCP routes, and three repetitions of the same 50 questions per pairing. The scorecard uses 150 scheduled evaluations per pairing, not 150 distinct questions.

[Machine-readable selection and provenance](ref-13-final-benchmark.json) · [Per-repetition CSV](ref-13-final-benchmark.csv)

## Final scores

| Model | Route | Right in each pass | Right / scheduled | Wrong | Scored | Unscored | Attempted |
|---|---|---|---:|---:|---:|---:|---:|
| GPT-6 Luna | Direct | 40 / 43 / 45 | 128/150 | 3 | 131 | 19 | 150/150 |
| GPT-6 Luna | BloodHound MCP | 47 / 49 / 49 | 145/150 | 2 | 147 | 3 | 150/150 |
| GPT-6 Luna | Armadin | 32 / 32 / 31 | 95/150 | 47 | 142 | 8 | 150/150 |
| GPT-6 Luna | Steven | 50 / 48 / 49 | 147/150 | 1 | 148 | 2 | 150/150 |
| GLM-5.3-Flash | Direct | 38 / 39 / 36 | 113/150 | 8 | 121 | 29 | 150/150 |
| GLM-5.3-Flash | BloodHound MCP | 23 / 26 / 24 | 73/150 | 42 | 115 | 35 | 150/150 |
| GLM-5.3-Flash | Armadin | 15 / 19 / 17 | 51/150 | 66 | 117 | 33 | 150/150 |
| GLM-5.3-Flash | Steven | 27 / 30 / 30 | 87/150 | 46 | 133 | 17 | 150/150 |
| DeepSeek-v4.1-Flash | Direct | 32 / 35 / 32 | 99/150 | 11 | 110 | 40 | 150/150 |
| DeepSeek-v4.1-Flash | BloodHound MCP | 28 / 27 / 27 | 82/150 | 57 | 139 | 11 | 150/150 |
| DeepSeek-v4.1-Flash | Armadin | 25 / 26 / 22 | 73/150 | 64 | 137 | 13 | 150/150 |
| DeepSeek-v4.1-Flash | Steven | 35 / 35 / 34 | 104/150 | 37 | 141 | 9 | 150/150 |
| Qwen3.8 Flash | Direct | 31 / 35 / 30 | 96/150 | 9 | 105 | 45 | 150/150 |
| Qwen3.8 Flash | BloodHound MCP | 28 / 26 / 28 | 82/150 | 52 | 134 | 16 | 150/150 |
| Qwen3.8 Flash | Armadin | 12 / 14 / 0 | 26/150 | 49 | 75 | 75 | 101/150 |
| Qwen3.8 Flash | Steven | 21 / 26 / 23 | 70/150 | 64 | 134 | 16 | 150/150 |

Right + wrong = scored; scored + unscored = scheduled. Unscored outcomes are not automatically scored wrong answers. Each question/repetition contributes once. Coverage is specific to a pairing: incomplete Qwen/Armadin coverage does not invalidate Steven or any other route. Cleanup and campaign lifecycle labels do not deduct points. Direct and MCP use different scoring contracts; this is not a universal model ranking.

## Token breakdown — same selected final runs

| Model | Route | Input tokens | Output tokens | Total tokens | Input share |
|---|---|---:|---:|---:|---:|
| GPT-6 Luna | Direct | 208,542 | 79,920 | 288,462 | 72.3% |
| GPT-6 Luna | BloodHound MCP | 10,314,102 | 197,051 | 10,511,153 | 98.1% |
| GPT-6 Luna | Armadin | 22,367,623 | 188,412 | 22,556,035 | 99.2% |
| GPT-6 Luna | Steven | 2,998,934 | 163,979 | 3,162,913 | 94.8% |
| GLM-5.3-Flash | Direct | 208,969 | 408,362 | 617,331 | 33.9% |
| GLM-5.3-Flash | BloodHound MCP | 10,874,025 | 660,945 | 11,534,970 | 94.3% |
| GLM-5.3-Flash | Armadin | 33,866,322 | 736,684 | 34,603,006 | 97.9% |
| GLM-5.3-Flash | Steven | 15,894,827 | 509,982 | 16,404,809 | 96.9% |
| DeepSeek-v4.1-Flash | Direct | 219,115 | 469,931 | 689,046 | 31.8% |
| DeepSeek-v4.1-Flash | BloodHound MCP | 12,935,470 | 415,444 | 13,350,914 | 96.9% |
| DeepSeek-v4.1-Flash | Armadin | 31,853,657 | 421,109 | 32,274,766 | 98.7% |
| DeepSeek-v4.1-Flash | Steven | 10,359,675 | 340,586 | 10,700,261 | 96.8% |
| Qwen3.8 Flash | Direct | 218,631 | 669,629 | 888,260 | 24.6% |
| Qwen3.8 Flash | BloodHound MCP | 19,911,729 | 784,212 | 20,695,941 | 96.2% |
| Qwen3.8 Flash | Armadin | 32,892,178 | 563,597 | 33,455,775 | 98.3% |
| Qwen3.8 Flash | Steven | 14,215,174 | 662,864 | 14,878,038 | 95.5% |

Usage includes recorded retry attempts within each selected repetition. The superseded whole repetition is excluded. These totals are not total project spending and do not establish dollar costs. Qwen/Armadin attempted 101/150 evaluations, so its raw token total is not a full-coverage cost comparison. No cache-token or billing breakdown is invented.

## Reproducible selection policy

GPT-6 Luna / Steven uses original repetitions 1 and 2, plus the final full rerun as replacement for the affected third repetition. The original third repetition is excluded wholesale—not combined with the best answers from the rerun. The final counts are 50, 48 and 49 correct: 147/150, with one scored wrong answer and two unscored outcomes retained from repetition 2. All 150 selected question slots were attempted; the selected records contain 152 attempt entries including retries.

The operator approved a full rerun of the affected 50-question repetition. The saved configuration describes it as covering 27 missed questions and repeating 23 prior attempts. The inspected saved defaults, MCP configurations and GPT fields match except repetition count; repetition count is itself included in the settings fingerprint. Thus the differing settings fingerprints alone do not establish a changed inference budget. Matching question, graph, comparator and task-binding identities were also checked. This is a documented derived presentation view, not a total emitted by a native merged report.

GLM and DeepSeek use their original three-repetition rows. Qwen3.8 Flash uses its three-repetition hosted matrix; it is not relabeled as the earlier local Qwen3.8-27B model. No result from one model or route fills another model or route.

### Source records

- [seed67-step1-six-models-3rep-3mcp-20260930](../../reports/runs/seed67-step1-six-models-3rep-3mcp-20260930/report.json), SHA-256 `fea50dd0b1069dd0c437571fb349a559dc1f8a912a41f10f55d6efc3c329ce8f`.
- [seed67-qwen38flash-gpt6luna-recovery-20261002](../../reports/runs/seed67-qwen38flash-gpt6luna-recovery-20261002/report.json), SHA-256 `8b117f98f960c5c0428d7a6157336db8a58f4276924797418a5a3f6990ba46f4`.

The JSON and CSV identify the exact source run, experiment and source repetition for each presentation repetition. Raw public reports and their historical model cards remain unchanged. Private coordination logs, raw task traces, credentials and sealed answer contents are not included.

Validation: 48 selected result rows, 16 model/route groups, and 2,400 unique selected question/repetition slots; aggregates independently recomputed from the source reports’ final question outcomes.
