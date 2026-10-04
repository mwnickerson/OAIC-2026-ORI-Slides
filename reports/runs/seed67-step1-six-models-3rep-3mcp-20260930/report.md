# ORI benchmark report

Status: **partial**.
Selection: `shared-question-v1`; question set fingerprint: `574c9e125c19797904ebee5e14749aab1404f7e555c9250c168f6ff434385dee`. Direct and MCP remain separate.

| Track | Experiment | Model | MCP | Rep | Correct / scheduled | Graded | Attempts | Tokens | Status |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | --- |
| direct | gpt-6-luna-nous-direct | gpt-6-luna-nous | — | 1 | 40/50 | 41 | 50 | 97117 | complete |
| direct | gpt-6-luna-nous-direct | gpt-6-luna-nous | — | 2 | 43/50 | 45 | 50 | 96680 | complete |
| direct | gpt-6-luna-nous-direct | gpt-6-luna-nous | — | 3 | 45/50 | 45 | 50 | 94665 | complete |
| mcp | gpt-6-luna-nous-mcp-bloodhound_mcp | gpt-6-luna-nous | bloodhound_mcp | 1 | 47/50 | 49 | 50 | 6822722 | partial |
| mcp | gpt-6-luna-nous-mcp-bloodhound_mcp | gpt-6-luna-nous | bloodhound_mcp | 2 | 49/50 | 49 | 50 | 1799201 | partial |
| mcp | gpt-6-luna-nous-mcp-bloodhound_mcp | gpt-6-luna-nous | bloodhound_mcp | 3 | 49/50 | 49 | 50 | 1889230 | partial |
| mcp | gpt-6-luna-nous-mcp-armadin | gpt-6-luna-nous | armadin | 1 | 32/50 | 48 | 50 | 7005483 | partial |
| mcp | gpt-6-luna-nous-mcp-armadin | gpt-6-luna-nous | armadin | 2 | 32/50 | 47 | 50 | 7387246 | partial |
| mcp | gpt-6-luna-nous-mcp-armadin | gpt-6-luna-nous | armadin | 3 | 31/50 | 47 | 50 | 8163306 | partial |
| mcp | gpt-6-luna-nous-mcp-steven_external | gpt-6-luna-nous | steven_external | 1 | 50/50 | 50 | 50 | 1009542 | partial; cleanup |
| mcp | gpt-6-luna-nous-mcp-steven_external | gpt-6-luna-nous | steven_external | 2 | 48/50 | 48 | 50 | 1096725 | partial; cleanup |
| mcp | gpt-6-luna-nous-mcp-steven_external | gpt-6-luna-nous | steven_external | 3 | 19/50 | 19 | 23 | 422376 | partial; cleanup |
| direct | glm-5.3-flash-nous-direct | glm-5.3-flash-nous | — | 1 | 38/50 | 41 | 50 | 225847 | complete |
| direct | glm-5.3-flash-nous-direct | glm-5.3-flash-nous | — | 2 | 39/50 | 43 | 50 | 196649 | complete |
| direct | glm-5.3-flash-nous-direct | glm-5.3-flash-nous | — | 3 | 36/50 | 37 | 50 | 194835 | complete |
| mcp | glm-5.3-flash-nous-mcp-bloodhound_mcp | glm-5.3-flash-nous | bloodhound_mcp | 1 | 23/50 | 40 | 50 | 4111391 | complete |
| mcp | glm-5.3-flash-nous-mcp-bloodhound_mcp | glm-5.3-flash-nous | bloodhound_mcp | 2 | 26/50 | 38 | 50 | 3627512 | complete |
| mcp | glm-5.3-flash-nous-mcp-bloodhound_mcp | glm-5.3-flash-nous | bloodhound_mcp | 3 | 24/50 | 37 | 50 | 3796067 | complete |
| mcp | glm-5.3-flash-nous-mcp-armadin | glm-5.3-flash-nous | armadin | 1 | 15/50 | 39 | 50 | 11290530 | partial |
| mcp | glm-5.3-flash-nous-mcp-armadin | glm-5.3-flash-nous | armadin | 2 | 19/50 | 41 | 50 | 12601108 | partial |
| mcp | glm-5.3-flash-nous-mcp-armadin | glm-5.3-flash-nous | armadin | 3 | 17/50 | 37 | 50 | 10711368 | partial |
| mcp | glm-5.3-flash-nous-mcp-steven_external | glm-5.3-flash-nous | steven_external | 1 | 27/50 | 45 | 50 | 3787279 | partial; cleanup |
| mcp | glm-5.3-flash-nous-mcp-steven_external | glm-5.3-flash-nous | steven_external | 2 | 30/50 | 45 | 50 | 3952995 | partial; cleanup |
| mcp | glm-5.3-flash-nous-mcp-steven_external | glm-5.3-flash-nous | steven_external | 3 | 30/50 | 43 | 50 | 8664535 | partial; cleanup |
| direct | deepseek-v4.1-flash-nous-direct | deepseek-v4.1-flash-nous | — | 1 | 32/50 | 37 | 50 | 189922 | complete |
| direct | deepseek-v4.1-flash-nous-direct | deepseek-v4.1-flash-nous | — | 2 | 35/50 | 38 | 50 | 235767 | complete |
| direct | deepseek-v4.1-flash-nous-direct | deepseek-v4.1-flash-nous | — | 3 | 32/50 | 35 | 50 | 263357 | complete |
| mcp | deepseek-v4.1-flash-nous-mcp-bloodhound_mcp | deepseek-v4.1-flash-nous | bloodhound_mcp | 1 | 28/50 | 46 | 50 | 3861916 | complete |
| mcp | deepseek-v4.1-flash-nous-mcp-bloodhound_mcp | deepseek-v4.1-flash-nous | bloodhound_mcp | 2 | 27/50 | 47 | 50 | 4771906 | complete |
| mcp | deepseek-v4.1-flash-nous-mcp-bloodhound_mcp | deepseek-v4.1-flash-nous | bloodhound_mcp | 3 | 27/50 | 46 | 50 | 4717092 | complete |
| mcp | deepseek-v4.1-flash-nous-mcp-armadin | deepseek-v4.1-flash-nous | armadin | 1 | 25/50 | 47 | 50 | 11567036 | partial |
| mcp | deepseek-v4.1-flash-nous-mcp-armadin | deepseek-v4.1-flash-nous | armadin | 2 | 26/50 | 44 | 50 | 9799910 | partial |
| mcp | deepseek-v4.1-flash-nous-mcp-armadin | deepseek-v4.1-flash-nous | armadin | 3 | 22/50 | 46 | 50 | 10907820 | partial |
| mcp | deepseek-v4.1-flash-nous-mcp-steven_external | deepseek-v4.1-flash-nous | steven_external | 1 | 35/50 | 47 | 50 | 3655699 | partial; cleanup |
| mcp | deepseek-v4.1-flash-nous-mcp-steven_external | deepseek-v4.1-flash-nous | steven_external | 2 | 35/50 | 47 | 50 | 3325836 | partial; cleanup |
| mcp | deepseek-v4.1-flash-nous-mcp-steven_external | deepseek-v4.1-flash-nous | steven_external | 3 | 34/50 | 47 | 50 | 3718726 | partial; cleanup |
| direct | qwen3.8-27b-q4km-direct | qwen3.8-27b-q4km | — | 1 | 6/50 | 6 | 50 | 9250 | partial; interrupted |
| direct | qwen3.8-27b-q4km-direct | qwen3.8-27b-q4km | — | 2 | 6/50 | 7 | 21 | 9932 | partial; interrupted |
| direct | qwen3.8-27b-q4km-direct | qwen3.8-27b-q4km | — | 3 | 0/50 | 0 | 0 | 0 | partial; interrupted |
| mcp | qwen3.8-27b-q4km-mcp-bloodhound_mcp | qwen3.8-27b-q4km | bloodhound_mcp | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | qwen3.8-27b-q4km-mcp-bloodhound_mcp | qwen3.8-27b-q4km | bloodhound_mcp | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | qwen3.8-27b-q4km-mcp-bloodhound_mcp | qwen3.8-27b-q4km | bloodhound_mcp | 3 | 0/50 | 0 | 0 | 0 | partial |
| mcp | qwen3.8-27b-q4km-mcp-armadin | qwen3.8-27b-q4km | armadin | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | qwen3.8-27b-q4km-mcp-armadin | qwen3.8-27b-q4km | armadin | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | qwen3.8-27b-q4km-mcp-armadin | qwen3.8-27b-q4km | armadin | 3 | 0/50 | 0 | 0 | 0 | partial |
| mcp | qwen3.8-27b-q4km-mcp-steven_external | qwen3.8-27b-q4km | steven_external | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | qwen3.8-27b-q4km-mcp-steven_external | qwen3.8-27b-q4km | steven_external | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | qwen3.8-27b-q4km-mcp-steven_external | qwen3.8-27b-q4km | steven_external | 3 | 0/50 | 0 | 0 | 0 | partial |
| direct | muse-glimmer-30b-direct | muse-glimmer-30b | — | 1 | 0/50 | 0 | 0 | 0 | partial |
| direct | muse-glimmer-30b-direct | muse-glimmer-30b | — | 2 | 0/50 | 0 | 0 | 0 | partial |
| direct | muse-glimmer-30b-direct | muse-glimmer-30b | — | 3 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-bloodhound_mcp | muse-glimmer-30b | bloodhound_mcp | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-bloodhound_mcp | muse-glimmer-30b | bloodhound_mcp | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-bloodhound_mcp | muse-glimmer-30b | bloodhound_mcp | 3 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-armadin | muse-glimmer-30b | armadin | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-armadin | muse-glimmer-30b | armadin | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-armadin | muse-glimmer-30b | armadin | 3 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-steven_external | muse-glimmer-30b | steven_external | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-steven_external | muse-glimmer-30b | steven_external | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | muse-glimmer-30b-mcp-steven_external | muse-glimmer-30b | steven_external | 3 | 0/50 | 0 | 0 | 0 | partial |
| direct | gemma-4-26b-it-qat-q4-0-64k-direct | gemma-4-26b-it-qat-q4-0-64k | — | 1 | 0/50 | 0 | 0 | 0 | partial |
| direct | gemma-4-26b-it-qat-q4-0-64k-direct | gemma-4-26b-it-qat-q4-0-64k | — | 2 | 0/50 | 0 | 0 | 0 | partial |
| direct | gemma-4-26b-it-qat-q4-0-64k-direct | gemma-4-26b-it-qat-q4-0-64k | — | 3 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-bloodhound_mcp | gemma-4-26b-it-qat-q4-0-64k | bloodhound_mcp | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-bloodhound_mcp | gemma-4-26b-it-qat-q4-0-64k | bloodhound_mcp | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-bloodhound_mcp | gemma-4-26b-it-qat-q4-0-64k | bloodhound_mcp | 3 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-armadin | gemma-4-26b-it-qat-q4-0-64k | armadin | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-armadin | gemma-4-26b-it-qat-q4-0-64k | armadin | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-armadin | gemma-4-26b-it-qat-q4-0-64k | armadin | 3 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-steven_external | gemma-4-26b-it-qat-q4-0-64k | steven_external | 1 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-steven_external | gemma-4-26b-it-qat-q4-0-64k | steven_external | 2 | 0/50 | 0 | 0 | 0 | partial |
| mcp | gemma-4-26b-it-qat-q4-0-64k-mcp-steven_external | gemma-4-26b-it-qat-q4-0-64k | steven_external | 3 | 0/50 | 0 | 0 | 0 | partial |

Runtime failures and missing task files remain in the scheduled denominator.
