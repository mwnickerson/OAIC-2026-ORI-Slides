# ORI benchmark report

Status: **partial**.
Selection: `shared-question-v1`; question set fingerprint: `574c9e125c19797904ebee5e14749aab1404f7e555c9250c168f6ff434385dee`. Direct and MCP remain separate.

| Track | Experiment | Model | MCP | Rep | Correct / scheduled | Graded | Attempts | Tokens | Status |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | --- |
| direct | glm-5.3-flash-nous-direct | glm-5.3-flash-nous | — | 1 | 39/50 | 41 | 50 | 210592 | complete |
| mcp | glm-5.3-flash-nous-mcp-bloodhound_mcp | glm-5.3-flash-nous | bloodhound_mcp | 1 | 28/50 | 44 | 50 | 3775636 | complete |
| mcp | glm-5.3-flash-nous-mcp-armadin | glm-5.3-flash-nous | armadin | 1 | 16/50 | 42 | 50 | 12953919 | partial |
| mcp | glm-5.3-flash-nous-mcp-steven_external | glm-5.3-flash-nous | steven_external | 1 | 31/50 | 47 | 50 | 2959137 | partial; cleanup |

Runtime failures and missing task files remain in the scheduled denominator.
