# ORI offline analysis · scored and unscored question ledger

The original ORI `state` field is preserved in `analysis.json` for audit. This human-facing report labels each row by scored coverage and its public outcome causes, rather than treating provider/infrastructure-affected slots as a model failure.

## Scope

Seven recent report-ready roots; 114 aggregate result rows; 5700 scheduled question slots. Repetitions and distinct task sets remain separate. All 21 cross-root comparisons did not pass the compatibility gate.

| Report root | Campaign status | Result rows | Scheduled | Attempted | Display categories |
|---|---|---:|---:|---:|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | partial | 13 | 650 | 601 | Output-validation issue · unscored, Provider/infra issue · unscored, Scores recorded · teardown note |
| seed67-step1-six-models-3rep-3mcp-20260930 | partial | 72 | 3600 | 1844 | Missing/interrupted · unscored, Output-validation issue · unscored, Provider/infra issue · unscored, Scores recorded · teardown note, Timeout-affected · unscored |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | partial | 4 | 200 | 200 | Output-validation issue · unscored, Provider/infra issue · unscored, Timeout-affected · unscored |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | partial | 8 | 400 | 373 | All scheduled scored, Output-validation issue · unscored, Provider/infra issue · unscored, Timeout-affected · unscored, Unscored · cause not established |
| glm53flash-shared-matrix-seed67-3mcp-20260929 | partial | 4 | 200 | 200 | Output-validation issue · unscored, Provider/infra issue · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | partial | 8 | 400 | 212 | Output-validation issue · unscored, Provider/infra issue · unscored, Timeout-affected · unscored |
| qwen3.8-json-rerun-2 | partial | 5 | 250 | 205 | Output-validation issue · unscored, Provider/infra issue · unscored |

## Scored right/wrong vs total scheduled

| Run | Model | Rep | Track | MCP | Right | Wrong | Scored | Scheduled | Unscored | Unscored causes | Attempt/error tallies | Display label |
|---|---|---:|---|---|---:|---:|---:|---:|---:|---|---|---|
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 1 | direct | Direct | 31 | 3 | 34 | 50 | 16 | OUTPUT_INVALID=13, QUERY_ERROR=3 | OUTPUT_INVALID=13, QUERY_ERROR=3 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 2 | direct | Direct | 35 | 2 | 37 | 50 | 13 | OUTPUT_INVALID=12, QUERY_ERROR=1 | OUTPUT_INVALID=12, QUERY_ERROR=1 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 3 | direct | Direct | 30 | 4 | 34 | 50 | 16 | OUTPUT_INVALID=12, QUERY_ERROR=4 | OUTPUT_INVALID=12, QUERY_ERROR=4 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 1 | mcp | bloodhound_mcp | 28 | 17 | 45 | 50 | 5 | OUTPUT_INVALID=5 | OUTPUT_INVALID=5 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 2 | mcp | bloodhound_mcp | 26 | 18 | 44 | 50 | 6 | OUTPUT_INVALID=6 | OUTPUT_INVALID=6 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 3 | mcp | bloodhound_mcp | 28 | 17 | 45 | 50 | 5 | OUTPUT_INVALID=5 | OUTPUT_INVALID=5 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 1 | mcp | armadin | 12 | 26 | 38 | 50 | 12 | INFRA_ERROR=6, OUTPUT_INVALID=6 | INFRA_ERROR=6, OUTPUT_INVALID=6 | Provider/infra issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 2 | mcp | armadin | 14 | 23 | 37 | 50 | 13 | INFRA_ERROR=9, OUTPUT_INVALID=4 | INFRA_ERROR=9, OUTPUT_INVALID=4 | Provider/infra issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 3 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | INFRA_ERROR=1, MISSING=49 | INFRA_ERROR=1, MISSING=49 | Provider/infra issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 1 | mcp | steven_external | 21 | 24 | 45 | 50 | 5 | OUTPUT_INVALID=5 | OUTPUT_INVALID=5 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 2 | mcp | steven_external | 26 | 19 | 45 | 50 | 5 | OUTPUT_INVALID=5 | OUTPUT_INVALID=5 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | qwen3.8-flash-nous | 3 | mcp | steven_external | 23 | 21 | 44 | 50 | 6 | OUTPUT_INVALID=6 | OUTPUT_INVALID=6 | Output-validation issue · unscored |
| seed67-qwen38flash-gpt6luna-recovery-20261002 | gpt-6-luna-nous | 1 | mcp | steven_external | 49 | 1 | 50 | 50 | 0 | none reported | none reported | Scores recorded · teardown note |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 1 | direct | Direct | 40 | 1 | 41 | 50 | 9 | QUERY_ERROR=3, QUERY_TIMEOUT=6 | QUERY_ERROR=3, QUERY_TIMEOUT=6 | Timeout-affected · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 2 | direct | Direct | 43 | 2 | 45 | 50 | 5 | QUERY_ERROR=4, QUERY_TIMEOUT=1 | QUERY_ERROR=4, QUERY_TIMEOUT=1 | Timeout-affected · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 3 | direct | Direct | 45 | 0 | 45 | 50 | 5 | QUERY_ERROR=3, QUERY_TIMEOUT=2 | QUERY_ERROR=3, QUERY_TIMEOUT=2 | Timeout-affected · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 1 | mcp | bloodhound_mcp | 47 | 2 | 49 | 50 | 1 | INFRA_ERROR=1 | INFRA_ERROR=1 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 2 | mcp | bloodhound_mcp | 49 | 0 | 49 | 50 | 1 | OUTPUT_INVALID=1 | OUTPUT_INVALID=1 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 3 | mcp | bloodhound_mcp | 49 | 0 | 49 | 50 | 1 | OUTPUT_INVALID=1 | OUTPUT_INVALID=1 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 1 | mcp | armadin | 32 | 16 | 48 | 50 | 2 | INFRA_ERROR=1, OUTPUT_INVALID=1 | INFRA_ERROR=1, OUTPUT_INVALID=1 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 2 | mcp | armadin | 32 | 15 | 47 | 50 | 3 | INFRA_ERROR=2, OUTPUT_INVALID=1 | INFRA_ERROR=2, OUTPUT_INVALID=1 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 3 | mcp | armadin | 31 | 16 | 47 | 50 | 3 | INFRA_ERROR=2, OUTPUT_INVALID=1 | INFRA_ERROR=2, OUTPUT_INVALID=1 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 1 | mcp | steven_external | 50 | 0 | 50 | 50 | 0 | none reported | none reported | Scores recorded · teardown note |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 2 | mcp | steven_external | 48 | 0 | 48 | 50 | 2 | INFRA_ERROR=1, OUTPUT_INVALID=1 | INFRA_ERROR=1, OUTPUT_INVALID=1 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gpt-6-luna-nous | 3 | mcp | steven_external | 19 | 0 | 19 | 50 | 31 | INFRA_ERROR=3, MISSING=27, OUTPUT_INVALID=1 | INFRA_ERROR=3, MISSING=27, OUTPUT_INVALID=1 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 1 | direct | Direct | 38 | 3 | 41 | 50 | 9 | OUTPUT_INVALID=5, QUERY_ERROR=4 | OUTPUT_INVALID=5, QUERY_ERROR=4 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 2 | direct | Direct | 39 | 4 | 43 | 50 | 7 | OUTPUT_INVALID=5, QUERY_ERROR=2 | OUTPUT_INVALID=5, QUERY_ERROR=2 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 3 | direct | Direct | 36 | 1 | 37 | 50 | 13 | OUTPUT_INVALID=9, QUERY_ERROR=4 | OUTPUT_INVALID=9, QUERY_ERROR=4 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 1 | mcp | bloodhound_mcp | 23 | 17 | 40 | 50 | 10 | OUTPUT_INVALID=10 | OUTPUT_INVALID=10 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 2 | mcp | bloodhound_mcp | 26 | 12 | 38 | 50 | 12 | OUTPUT_INVALID=12 | OUTPUT_INVALID=12 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 3 | mcp | bloodhound_mcp | 24 | 13 | 37 | 50 | 13 | OUTPUT_INVALID=13 | OUTPUT_INVALID=13 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 1 | mcp | armadin | 15 | 24 | 39 | 50 | 11 | INFRA_ERROR=2, OUTPUT_INVALID=9 | INFRA_ERROR=2, OUTPUT_INVALID=9 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 2 | mcp | armadin | 19 | 22 | 41 | 50 | 9 | INFRA_ERROR=2, OUTPUT_INVALID=7 | INFRA_ERROR=2, OUTPUT_INVALID=7 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 3 | mcp | armadin | 17 | 20 | 37 | 50 | 13 | INFRA_ERROR=3, OUTPUT_INVALID=10 | INFRA_ERROR=3, OUTPUT_INVALID=10 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 1 | mcp | steven_external | 27 | 18 | 45 | 50 | 5 | INFRA_ERROR=1, OUTPUT_INVALID=4 | INFRA_ERROR=1, OUTPUT_INVALID=4 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 2 | mcp | steven_external | 30 | 15 | 45 | 50 | 5 | INFRA_ERROR=1, OUTPUT_INVALID=4 | INFRA_ERROR=1, OUTPUT_INVALID=4 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | glm-5.3-flash-nous | 3 | mcp | steven_external | 30 | 13 | 43 | 50 | 7 | OUTPUT_INVALID=7 | OUTPUT_INVALID=7 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 1 | direct | Direct | 32 | 5 | 37 | 50 | 13 | OUTPUT_INVALID=3, QUERY_ERROR=5, TASK_TIMEOUT=5 | OUTPUT_INVALID=3, QUERY_ERROR=5, TASK_TIMEOUT=5 | Timeout-affected · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 2 | direct | Direct | 35 | 3 | 38 | 50 | 12 | OUTPUT_INVALID=7, QUERY_ERROR=5 | OUTPUT_INVALID=7, QUERY_ERROR=5 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 3 | direct | Direct | 32 | 3 | 35 | 50 | 15 | OUTPUT_INVALID=10, QUERY_ERROR=5 | OUTPUT_INVALID=10, QUERY_ERROR=5 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 1 | mcp | bloodhound_mcp | 28 | 18 | 46 | 50 | 4 | OUTPUT_INVALID=4 | OUTPUT_INVALID=4 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 2 | mcp | bloodhound_mcp | 27 | 20 | 47 | 50 | 3 | OUTPUT_INVALID=3 | OUTPUT_INVALID=3 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 3 | mcp | bloodhound_mcp | 27 | 19 | 46 | 50 | 4 | OUTPUT_INVALID=4 | OUTPUT_INVALID=4 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 1 | mcp | armadin | 25 | 22 | 47 | 50 | 3 | INFRA_ERROR=1, OUTPUT_INVALID=2 | INFRA_ERROR=1, OUTPUT_INVALID=2 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 2 | mcp | armadin | 26 | 18 | 44 | 50 | 6 | INFRA_ERROR=2, OUTPUT_INVALID=4 | INFRA_ERROR=2, OUTPUT_INVALID=4 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 3 | mcp | armadin | 22 | 24 | 46 | 50 | 4 | INFRA_ERROR=2, OUTPUT_INVALID=2 | INFRA_ERROR=2, OUTPUT_INVALID=2 | Provider/infra issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 1 | mcp | steven_external | 35 | 12 | 47 | 50 | 3 | OUTPUT_INVALID=3 | OUTPUT_INVALID=3 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 2 | mcp | steven_external | 35 | 12 | 47 | 50 | 3 | OUTPUT_INVALID=3 | OUTPUT_INVALID=3 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | deepseek-v4.1-flash-nous | 3 | mcp | steven_external | 34 | 13 | 47 | 50 | 3 | OUTPUT_INVALID=3 | OUTPUT_INVALID=3 | Output-validation issue · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 1 | direct | Direct | 6 | 0 | 6 | 50 | 44 | TASK_TIMEOUT=44 | TASK_TIMEOUT=44 | Timeout-affected · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 2 | direct | Direct | 6 | 1 | 7 | 50 | 43 | INTERRUPTED=1, MISSING=29, TASK_TIMEOUT=13 | INTERRUPTED=1, MISSING=29, TASK_TIMEOUT=13 | Timeout-affected · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 3 | direct | Direct | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 1 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 2 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 3 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 1 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 2 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 3 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 1 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 2 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | qwen3.8-27b-q4km | 3 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 1 | direct | Direct | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 2 | direct | Direct | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 3 | direct | Direct | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 1 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 2 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 3 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 1 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 2 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 3 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 1 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 2 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | muse-glimmer-30b | 3 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 1 | direct | Direct | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 2 | direct | Direct | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 3 | direct | Direct | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 1 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 2 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 3 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 1 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 2 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 3 | mcp | armadin | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 1 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 2 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| seed67-step1-six-models-3rep-3mcp-20260930 | gemma-4-26b-it-qat-q4-0-64k | 3 | mcp | steven_external | 0 | 0 | 0 | 50 | 50 | MISSING=50 | MISSING=50 | Missing/interrupted · unscored |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | deepseek-v4.1-flash-nous | 1 | direct | Direct | 29 | 4 | 33 | 50 | 17 | QUERY_ERROR=4, QUERY_TIMEOUT=1, TASK_TIMEOUT=12 | QUERY_ERROR=4, QUERY_TIMEOUT=1, TASK_TIMEOUT=12 | Timeout-affected · unscored |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | deepseek-v4.1-flash-nous | 1 | mcp | bloodhound_mcp | 38 | 7 | 45 | 50 | 5 | INFRA_ERROR=1, OUTPUT_INVALID=4 | INFRA_ERROR=1, OUTPUT_INVALID=4 | Provider/infra issue · unscored |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | deepseek-v4.1-flash-nous | 1 | mcp | armadin | 23 | 24 | 47 | 50 | 3 | INFRA_ERROR=1, OUTPUT_INVALID=2 | INFRA_ERROR=1, OUTPUT_INVALID=2 | Provider/infra issue · unscored |
| deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929 | deepseek-v4.1-flash-nous | 1 | mcp | steven_external | 36 | 11 | 47 | 50 | 3 | OUTPUT_INVALID=3 | OUTPUT_INVALID=3 | Output-validation issue · unscored |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | gpt-6-luna-nous | 1 | direct | Direct | 46 | 1 | 47 | 50 | 3 | QUERY_ERROR=1, QUERY_TIMEOUT=2 | QUERY_ERROR=1, QUERY_TIMEOUT=2 | Timeout-affected · unscored |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | gpt-6-luna-nous | 1 | mcp | bloodhound_mcp | 49 | 1 | 50 | 50 | 0 | none reported | none reported | All scheduled scored |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | gpt-6-luna-nous | 1 | mcp | armadin | 30 | 19 | 49 | 50 | 1 | INFRA_ERROR=1 | INFRA_ERROR=1 | Provider/infra issue · unscored |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | gpt-6-luna-nous | 1 | mcp | steven_external | 48 | 1 | 49 | 50 | 1 | OUTPUT_INVALID=1 | OUTPUT_INVALID=1 | Output-validation issue · unscored |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | gpt-5.6-luna-nous | 1 | direct | Direct | 42 | 3 | 45 | 50 | 5 | QUERY_ERROR=5 | QUERY_ERROR=5 | Unscored · cause not established |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | gpt-5.6-luna-nous | 1 | mcp | bloodhound_mcp | 18 | 1 | 19 | 50 | 31 | INFRA_ERROR=3, MISSING=27, OUTPUT_INVALID=1 | INFRA_ERROR=3, MISSING=27, OUTPUT_INVALID=1 | Provider/infra issue · unscored |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | gpt-5.6-luna-nous | 1 | mcp | armadin | 35 | 13 | 48 | 50 | 2 | INFRA_ERROR=1, OUTPUT_INVALID=1 | INFRA_ERROR=1, OUTPUT_INVALID=1 | Provider/infra issue · unscored |
| luna-nous-shared-matrix-seed67-3mcp-20260929 | gpt-5.6-luna-nous | 1 | mcp | steven_external | 44 | 3 | 47 | 50 | 3 | INFRA_ERROR=1, OUTPUT_INVALID=2 | INFRA_ERROR=1, OUTPUT_INVALID=2 | Provider/infra issue · unscored |
| glm53flash-shared-matrix-seed67-3mcp-20260929 | glm-5.3-flash-nous | 1 | direct | Direct | 39 | 2 | 41 | 50 | 9 | OUTPUT_INVALID=7, QUERY_ERROR=2 | OUTPUT_INVALID=7, QUERY_ERROR=2 | Output-validation issue · unscored |
| glm53flash-shared-matrix-seed67-3mcp-20260929 | glm-5.3-flash-nous | 1 | mcp | bloodhound_mcp | 28 | 16 | 44 | 50 | 6 | OUTPUT_INVALID=6 | OUTPUT_INVALID=6 | Output-validation issue · unscored |
| glm53flash-shared-matrix-seed67-3mcp-20260929 | glm-5.3-flash-nous | 1 | mcp | armadin | 16 | 26 | 42 | 50 | 8 | INFRA_ERROR=2, OUTPUT_INVALID=6 | INFRA_ERROR=2, OUTPUT_INVALID=6 | Provider/infra issue · unscored |
| glm53flash-shared-matrix-seed67-3mcp-20260929 | glm-5.3-flash-nous | 1 | mcp | steven_external | 31 | 16 | 47 | 50 | 3 | OUTPUT_INVALID=3 | OUTPUT_INVALID=3 | Output-validation issue · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | glm-5.3-flash-nous | 1 | direct | Direct | 44 | 0 | 44 | 50 | 6 | OUTPUT_INVALID=2, QUERY_ERROR=3, QUERY_TIMEOUT=1 | OUTPUT_INVALID=2, QUERY_ERROR=3, QUERY_TIMEOUT=1 | Timeout-affected · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | glm-5.3-flash-nous | 1 | mcp | bloodhound_mcp | 26 | 17 | 43 | 50 | 7 | OUTPUT_INVALID=7 | OUTPUT_INVALID=7 | Output-validation issue · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | qwen3.8-flash-nous | 1 | direct | Direct | 31 | 2 | 33 | 50 | 17 | OUTPUT_INVALID=11, QUERY_ERROR=6 | OUTPUT_INVALID=11, QUERY_ERROR=6 | Output-validation issue · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | qwen3.8-flash-nous | 1 | mcp | bloodhound_mcp | 24 | 20 | 44 | 50 | 6 | OUTPUT_INVALID=6 | OUTPUT_INVALID=6 | Output-validation issue · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | gpt-6-luna | 1 | direct | Direct | 0 | 0 | 0 | 50 | 50 | INFRA_ERROR=3, MISSING=47 | INFRA_ERROR=3, MISSING=47 | Provider/infra issue · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | gpt-6-luna | 1 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | INFRA_ERROR=3, MISSING=47 | INFRA_ERROR=3, MISSING=47 | Provider/infra issue · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | gpt-5.6-luna | 1 | direct | Direct | 0 | 0 | 0 | 50 | 50 | INFRA_ERROR=3, MISSING=47 | INFRA_ERROR=3, MISSING=47 | Provider/infra issue · unscored |
| shared-matrix-seed67-bloodhound-nous-codex-20260928 | gpt-5.6-luna | 1 | mcp | bloodhound_mcp | 0 | 0 | 0 | 50 | 50 | INFRA_ERROR=3, MISSING=47 | INFRA_ERROR=3, MISSING=47 | Provider/infra issue · unscored |
| qwen3.8-json-rerun-2 | qwen3.8-27b-q4km | 1 | direct | Direct | 29 | 2 | 31 | 50 | 19 | OUTPUT_INVALID=17, QUERY_ERROR=2 | OUTPUT_INVALID=17, QUERY_ERROR=2 | Output-validation issue · unscored |
| qwen3.8-json-rerun-2 | qwen3.8-27b-q4km | 1 | mcp | bloodhound_mcp | 34 | 10 | 44 | 50 | 6 | INFRA_ERROR=2, OUTPUT_INVALID=4 | INFRA_ERROR=2, OUTPUT_INVALID=4 | Provider/infra issue · unscored |
| qwen3.8-json-rerun-2 | qwen3.8-27b-q4km | 1 | mcp | mordavid | 2 | 0 | 2 | 50 | 48 | INFRA_ERROR=3, MISSING=45 | INFRA_ERROR=3, MISSING=45 | Provider/infra issue · unscored |
| qwen3.8-json-rerun-2 | qwen3.8-27b-q4km | 1 | mcp | armadin | 20 | 16 | 36 | 50 | 14 | INFRA_ERROR=5, OUTPUT_INVALID=7, TASK_TIMEOUT=2 | INFRA_ERROR=5, OUTPUT_INVALID=7, TASK_TIMEOUT=2 | Provider/infra issue · unscored |
| qwen3.8-json-rerun-2 | qwen3.8-27b-q4km | 1 | mcp | steven_external | 35 | 9 | 44 | 50 | 6 | INFRA_ERROR=1, OUTPUT_INVALID=5 | INFRA_ERROR=1, OUTPUT_INVALID=5 | Provider/infra issue · unscored |

Question counts come from ORI `graded` and public question-result `reasoning_correct`: right + wrong = scored; unscored = scheduled − scored. Unscored outcome causes are counted from public question rows. Aggregate attempt/error tallies are shown separately and may reflect retries/events, not one unique failed question per count.

## Provider/infrastructure note

The Qwen3.8 Flash/Armadin public rows show reason-specific coverage and cause labels. The HTTP-400 mechanism below is operator-supplied; task-attempt files were not reopened.

Operator-supplied: 34 HTTP 400 responses followed successful MCP tool-call turns; 26 were associated with final INFRA_ERROR tasks and 8 in records that later completed. Repetition 3 had 49 unexecuted scheduled questions. A repeated position-9 event followed a 3,710,830-character `analyze_group_permissions` result and an estimated 4.49 MB reconstructed messages-plus-tool-schemas core (not a complete HTTP payload). Smaller failures and larger successes mean no single request-size threshold is established; response body was not saved, so exact rejection reason is unknown. Operator reports broad PROVIDER_PROTOCOL classification. Treat as provider/protocol outcomes, not reasoning errors. Steven External cleanup is a separate teardown issue.

## API usage and cost

Input/output token counters are present in 114/114 rows. Recorded API costs are present in 0/114. Cache-token categories in public reports: none. Cost is not recorded/not computed, not zero; no estimates are invented.

## Interpretation / provenance

Infrastructure/protocol issue, timeout, output-validation issue, incomplete/missing work, interruption, and teardown note are presentation labels based on public outcome data. They are not diagnoses of model reasoning ability. `analysis.json` preserves the raw ORI result state and source references. No private task records, transcripts, credentials, or sealed expected answers were opened.

See `question-scoring-ledger.json` for the machine-readable question-scored breakdown; `model-cards/` has one card per model/MCP pairing with per-repetition right/wrong/unscored counts, outcome causes, token counts, and unavailable cost labels.


## Public source links

- [Raw aggregate analysis](analysis.json) — historical ORI lifecycle status is retained.
- [Question scoring ledger](question-scoring-ledger.json) — final public outcome counts, distinct from retry/error tallies.
- [Presentation status ledger](presentation-status-ledger.json) — coverage/cause labels.
- [Model cards](model-cards/) — full per-repetition Markdown tables and compact SVG/PNG previews.

The SVG/PNG cards are compact previews of up to four rows; some cause lists are shortened. Use the Markdown cards or JSON ledgers for complete rows, causes, run identities, and repetitions.

Original public run reports (retained unchanged):

- [seed67-qwen38flash-gpt6luna-recovery-20261002](../runs/seed67-qwen38flash-gpt6luna-recovery-20261002/report.json)
- [seed67-step1-six-models-3rep-3mcp-20260930](../runs/seed67-step1-six-models-3rep-3mcp-20260930/report.json)
- [deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929](../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929/report.json)
- [luna-nous-shared-matrix-seed67-3mcp-20260929](../runs/luna-nous-shared-matrix-seed67-3mcp-20260929/report.json)
- [glm53flash-shared-matrix-seed67-3mcp-20260929](../runs/glm53flash-shared-matrix-seed67-3mcp-20260929/report.json)
- [shared-matrix-seed67-bloodhound-nous-codex-20260928](../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928/report.json)
- [qwen3.8-json-rerun-2](../runs/qwen3.8-json-rerun-2/report.json)
