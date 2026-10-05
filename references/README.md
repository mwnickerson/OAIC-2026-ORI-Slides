# References and result sources

The final scorecard and token breakdown use reference **13**, a reproducible per-repetition selection derived from the unchanged native reports. References 1–12 retain their source identities for historical context and technical exhibits. Historical lifecycle fields are not benchmark correctness verdicts.

| Reference | Source | Current use | File |
|---|---|---|---|
| [1] | GLM-5.3-Flash, September 29–30 | Historical supporting results | [ref-01-glm53.csv](data/ref-01-glm53.csv) |
| [2] | GPT-6 Luna and GPT-5.6 Luna, September 29–30 | Historical supporting results | [ref-02-luna.csv](data/ref-02-luna.csv) |
| [3] | DeepSeek-v4.1-Flash, September 29–30 | Historical supporting results | [ref-03-deepseek.csv](data/ref-03-deepseek.csv) |
| [4] | September 28 hosted results and usage | Historical supporting results | [ref-04-hosted.csv](data/ref-04-hosted.csv) |
| [5] | Three-repetition seed-67 native campaign | Source for final selection [13] | [ref-05-three-repetitions.csv](data/ref-05-three-repetitions.csv) |
| [6] | Qwen3.8 Flash matrix and final GPT-6 Steven pass | Source for final selection [13] | [ref-06-recovery.csv](data/ref-06-recovery.csv) |
| [7] | Sanitized HTTP 400 records | Supporting request diagnostics | [ref-07-http-errors.csv](data/ref-07-http-errors.csv) |
| [8] | Local Qwen five-route aggregate | Historical supporting results | [ref-08-local-qwen.csv](data/ref-08-local-qwen.csv) |
| [9] | Saved tool-output size and reconstructed request core | Slide 27 | [ref-09-request-size.json](data/ref-09-request-size.json) |
| [10] | Native-report right/wrong/scored/unscored ledger | Scoring methodology and backing detail | [Question scoring ledger](../reports/ori-recent-runs-2026-10-04/question-scoring-ledger.json) |
| [11] | Native-report coverage and status labels | Backing detail | [Presentation status ledger](../reports/ori-recent-runs-2026-10-04/presentation-status-ledger.json) |
| [12] | Seed streams, generation and task compilation | Slide 19 | [Seed mechanics](data/ref-12-seed-mechanics.md) |
| [13] | Final three-run scores and input/output token usage | Slides 25–26 | [Explanation and tables](data/ref-13-final-benchmark.md) · [JSON](data/ref-13-final-benchmark.json) · [CSV](data/ref-13-final-benchmark.csv) |

Reference 13 selects three repetitions per model/route. GPT-6 Luna/Steven uses original repetitions 1 and 2 plus the full rerun replacing repetition 3: 147/150 correct, one wrong, two unscored. It does not reuse rerun answers to repair other repetitions or mix original and rerun answers into a best-of result. Qwen Flash is kept distinct from the earlier local Qwen model. The JSON records source runs, source repetitions, hashes and scoring/usage definitions.

References 1–6 and 8 are byte-identical aggregate CSVs; 7 and 9 are sanitized derived diagnostics. All seven native campaigns and historical model cards remain under [reports](../reports/README.md) and in the [dated history](../history/2026-10-04/README.md). Those records are not additional observations or the final selected presentation table.

Reference 9 measures retained content, not raw tool content published here. The approximately 4.49 MB figure is reconstructed compact JSON containing saved messages and 97 tool schemas—not an HTTP wire capture, a token count or a proven provider threshold. The rejection body and exact cause were not saved.

## Project and article links from the slides

- https://github.com/MorDavid/BloodHound-MCP-AI
- https://github.com/SpecterOps/BloodHound
- https://github.com/armadin-public/bloodhound-mcp-server
- https://github.com/mwnickerson/bloodhound_mcp
- https://github.com/stevenyu113228/BloodHound-MCP
- https://specterops.io/blog/2025/06/04/chatting-with-your-attack-paths-an-mcp-for-bloodhound
- https://www.armadin.com/blog-posts/automating-the-operator-integrating-llms-into-offensive-security-workflows
