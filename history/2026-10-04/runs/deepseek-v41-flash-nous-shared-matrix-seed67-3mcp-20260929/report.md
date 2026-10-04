# ORI benchmark report

Status: **partial**.
Selection: `shared-question-v1`; question set fingerprint: `574c9e125c19797904ebee5e14749aab1404f7e555c9250c168f6ff434385dee`. Direct and MCP remain separate.

| Track | Experiment | Model | MCP | Rep | Correct / scheduled | Graded | Attempts | Tokens | Status |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | --- |
| direct | deepseek-v4.1-flash-nous-direct | deepseek-v4.1-flash-nous | — | 1 | 29/50 | 33 | 50 | 163768 | complete |
| mcp | deepseek-v4.1-flash-nous-mcp-bloodhound_mcp | deepseek-v4.1-flash-nous | bloodhound_mcp | 1 | 38/50 | 45 | 50 | 3847681 | partial |
| mcp | deepseek-v4.1-flash-nous-mcp-armadin | deepseek-v4.1-flash-nous | armadin | 1 | 23/50 | 47 | 50 | 10916938 | partial |
| mcp | deepseek-v4.1-flash-nous-mcp-steven_external | deepseek-v4.1-flash-nous | steven_external | 1 | 36/50 | 47 | 50 | 3315113 | partial; cleanup |

Runtime failures and missing task files remain in the scheduled denominator.
