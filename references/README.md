# References and result sources

The numbered files below are the evidence cited on the slides' References page. References 1–6 and 8 are byte-identical aggregate CSVs; references 7 and 9 are sanitized, derived diagnostics, not additional campaigns.

| Reference | Source | Slide | File |
|---|---|---|---|
| [1] | GLM-5.3-Flash: seed 67, September 29–30 | 27 | [ref-01-glm53.csv](data/ref-01-glm53.csv) |
| [2] | GPT-6 Luna and GPT-5.6 Luna: seed 67, September 29–30 | 27 | [ref-02-luna.csv](data/ref-02-luna.csv) |
| [3] | DeepSeek-v4.1-Flash: seed 67, September 29–30 | 27 | [ref-03-deepseek.csv](data/ref-03-deepseek.csv) |
| [4] | September 28 hosted campaign: results, login-provider cutoffs and usage | 26, 28 | [ref-04-hosted.csv](data/ref-04-hosted.csv) |
| [5] | Three-repetition seed-67 campaign: interrupted | 29 | [ref-05-three-repetitions.csv](data/ref-05-three-repetitions.csv) |
| [6] | Qwen3.8 Flash and GPT-6 Luna recovery: partial | 30 | [ref-06-recovery.csv](data/ref-06-recovery.csv) |
| [7] | Sanitized provider HTTP 400 failure summary | 31 | [ref-07-http-errors.csv](data/ref-07-http-errors.csv) |
| [8] | Local Qwen five-route aggregate: scores, attempts and partial states | 25 | [ref-08-local-qwen.csv](data/ref-08-local-qwen.csv) |
| [9] | Retained tool-output size, reconstructed request core and historical failures | 31 | [ref-09-request-size.json](data/ref-09-request-size.json) |

All seven recent campaigns, including the local Qwen rerun, are available under [reports/runs](../reports/runs/). The [recent-run analysis and model cards](../reports/ori-recent-runs-2026-10-04/) retain their run/cohort and repetition boundaries. The copies here are citation aliases, not additional observations.

Reference 9 independently checks retained-content sizes; it does not include raw tool content. The 4.49 MB figure describes compact JSON containing saved messages and 97 tool schemas, not a captured full request or HTTP wire measurement. The rejection body, any provider size/context limit and the cause of HTTP 400 remain unknown. Historical attempts and latest task outcomes are different counts.

## Project and article links from the slides

- https://github.com/MorDavid/BloodHound-MCP-AI
- https://github.com/SpecterOps/BloodHound
- https://github.com/armadin-public/bloodhound-mcp-server
- https://github.com/mwnickerson/bloodhound_mcp
- https://github.com/stevenyu113228/BloodHound-MCP
- https://specterops.io/blog/2025/06/04/chatting-with-your-attack-paths-an-mcp-for-bloodhound
- https://www.armadin.com/blog-posts/automating-the-operator-integrating-llms-into-offensive-security-workflows
