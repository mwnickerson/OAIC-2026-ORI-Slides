# ORI benchmark report

Status: **partial**.
Selection: `shared-question-v1`; question set fingerprint: `574c9e125c19797904ebee5e14749aab1404f7e555c9250c168f6ff434385dee`. Direct and MCP remain separate.

| Track | Experiment | Model | MCP | Rep | Correct / scheduled | Graded | Attempts | Tokens | Status |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | --- |
| direct | glm-5.3-flash-nous-direct | glm-5.3-flash-nous | — | 1 | 44/50 | 44 | 50 | 198912 | complete |
| mcp | glm-5.3-flash-nous-mcp-bloodhound_mcp | glm-5.3-flash-nous | bloodhound_mcp | 1 | 26/50 | 43 | 50 | 4897552 | complete |
| direct | qwen3.8-flash-nous-direct | qwen3.8-flash-nous | — | 1 | 31/50 | 33 | 50 | 277098 | complete |
| mcp | qwen3.8-flash-nous-mcp-bloodhound_mcp | qwen3.8-flash-nous | bloodhound_mcp | 1 | 24/50 | 44 | 50 | 6239067 | complete |
| direct | gpt-6-luna-direct | gpt-6-luna | — | 1 | 0/50 | 0 | 3 | 0 | partial; infrastructure_cutoff |
| mcp | gpt-6-luna-mcp-bloodhound_mcp | gpt-6-luna | bloodhound_mcp | 1 | 0/50 | 0 | 3 | 0 | partial; infrastructure_cutoff |
| direct | gpt-5.6-luna-direct | gpt-5.6-luna | — | 1 | 0/50 | 0 | 3 | 0 | partial; infrastructure_cutoff |
| mcp | gpt-5.6-luna-mcp-bloodhound_mcp | gpt-5.6-luna | bloodhound_mcp | 1 | 0/50 | 0 | 3 | 0 | partial; infrastructure_cutoff |

Runtime failures and missing task files remain in the scheduled denominator.
