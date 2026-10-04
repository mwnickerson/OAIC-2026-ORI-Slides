# ORI benchmark report

Status: **partial**.
Selection: `shared-question-v1`; question set fingerprint: `574c9e125c19797904ebee5e14749aab1404f7e555c9250c168f6ff434385dee`. Direct and MCP remain separate.

| Track | Experiment | Model | MCP | Rep | Correct / scheduled | Graded | Attempts | Tokens | Status |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | --- |
| direct | gpt-6-luna-nous-direct | gpt-6-luna-nous | — | 1 | 46/50 | 47 | 50 | 99086 | complete |
| mcp | gpt-6-luna-nous-mcp-bloodhound_mcp | gpt-6-luna-nous | bloodhound_mcp | 1 | 49/50 | 50 | 53 | 2148022 | complete |
| mcp | gpt-6-luna-nous-mcp-armadin | gpt-6-luna-nous | armadin | 1 | 30/50 | 49 | 51 | 7529004 | partial |
| mcp | gpt-6-luna-nous-mcp-steven_external | gpt-6-luna-nous | steven_external | 1 | 48/50 | 49 | 50 | 1146791 | partial; cleanup |
| direct | gpt-5.6-luna-nous-direct | gpt-5.6-luna-nous | — | 1 | 42/50 | 45 | 50 | 94933 | complete |
| mcp | gpt-5.6-luna-nous-mcp-bloodhound_mcp | gpt-5.6-luna-nous | bloodhound_mcp | 1 | 18/50 | 19 | 26 | 767914 | partial; cleanup |
| mcp | gpt-5.6-luna-nous-mcp-armadin | gpt-5.6-luna-nous | armadin | 1 | 35/50 | 48 | 50 | 7212675 | partial |
| mcp | gpt-5.6-luna-nous-mcp-steven_external | gpt-5.6-luna-nous | steven_external | 1 | 44/50 | 47 | 53 | 1808238 | partial; cleanup |

Runtime failures and missing task files remain in the scheduled denominator.
