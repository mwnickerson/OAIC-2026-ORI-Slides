# ORI benchmark report

Status: **partial**.
Selection: `shared-question-v1`; question set fingerprint: `574c9e125c19797904ebee5e14749aab1404f7e555c9250c168f6ff434385dee`. Direct and MCP remain separate.

| Track | Experiment | Model | MCP | Rep | Correct / scheduled | Graded | Attempts | Tokens | Status |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | --- |
| direct | qwen3.8-27b-q4km-direct | qwen3.8-27b-q4km | — | 1 | 29/50 | 31 | 50 | 312989 | complete |
| mcp | qwen3.8-27b-q4km-mcp-bloodhound_mcp | qwen3.8-27b-q4km | bloodhound_mcp | 1 | 34/50 | 44 | 50 | 4258406 | partial |
| mcp | qwen3.8-27b-q4km-mcp-mordavid | qwen3.8-27b-q4km | mordavid | 1 | 2/50 | 2 | 5 | 93545 | partial; infrastructure_cutoff |
| mcp | qwen3.8-27b-q4km-mcp-armadin | qwen3.8-27b-q4km | armadin | 1 | 20/50 | 36 | 50 | 9124072 | partial |
| mcp | qwen3.8-27b-q4km-mcp-steven_external | qwen3.8-27b-q4km | steven_external | 1 | 35/50 | 44 | 50 | 3606565 | partial; cleanup |

Runtime failures and missing task files remain in the scheduled denominator.
