# ORI benchmark report

Status: **partial**.
Selection: `shared-question-v1`; question set fingerprint: `574c9e125c19797904ebee5e14749aab1404f7e555c9250c168f6ff434385dee`. Direct and MCP remain separate.

| Track | Experiment | Model | MCP | Rep | Correct / scheduled | Graded | Attempts | Tokens | Status |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | --- |
| direct | qwen3.8-flash-nous-direct | qwen3.8-flash-nous | — | 1 | 31/50 | 34 | 50 | 296630 | complete |
| direct | qwen3.8-flash-nous-direct | qwen3.8-flash-nous | — | 2 | 35/50 | 37 | 50 | 295142 | complete |
| direct | qwen3.8-flash-nous-direct | qwen3.8-flash-nous | — | 3 | 30/50 | 34 | 50 | 296488 | complete |
| mcp | qwen3.8-flash-nous-mcp-bloodhound_mcp | qwen3.8-flash-nous | bloodhound_mcp | 1 | 28/50 | 45 | 50 | 5460557 | complete |
| mcp | qwen3.8-flash-nous-mcp-bloodhound_mcp | qwen3.8-flash-nous | bloodhound_mcp | 2 | 26/50 | 44 | 50 | 9192589 | complete |
| mcp | qwen3.8-flash-nous-mcp-bloodhound_mcp | qwen3.8-flash-nous | bloodhound_mcp | 3 | 28/50 | 45 | 50 | 6042795 | complete |
| mcp | qwen3.8-flash-nous-mcp-armadin | qwen3.8-flash-nous | armadin | 1 | 12/50 | 38 | 60 | 17051373 | partial; infrastructure_cutoff |
| mcp | qwen3.8-flash-nous-mcp-armadin | qwen3.8-flash-nous | armadin | 2 | 14/50 | 37 | 59 | 16342164 | partial; infrastructure_cutoff |
| mcp | qwen3.8-flash-nous-mcp-armadin | qwen3.8-flash-nous | armadin | 3 | 0/50 | 0 | 1 | 62238 | partial; infrastructure_cutoff |
| mcp | qwen3.8-flash-nous-mcp-steven_external | qwen3.8-flash-nous | steven_external | 1 | 21/50 | 45 | 51 | 5300328 | partial; cleanup |
| mcp | qwen3.8-flash-nous-mcp-steven_external | qwen3.8-flash-nous | steven_external | 2 | 26/50 | 45 | 50 | 5308349 | partial; cleanup |
| mcp | qwen3.8-flash-nous-mcp-steven_external | qwen3.8-flash-nous | steven_external | 3 | 23/50 | 44 | 50 | 4269361 | partial; cleanup |
| mcp | gpt-6-luna-nous-mcp-steven_external | gpt-6-luna-nous | steven_external | 1 | 49/50 | 50 | 52 | 1056646 | partial; cleanup |

Runtime failures and missing task files remain in the scheduled denominator.
