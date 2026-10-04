# Campaign reports

The seven campaigns below are the sources of the [recent-run analysis](ori-recent-runs-2026-10-04/analysis.md). Each directory includes its original report Markdown, public report JSON, aggregate CSV, and lifecycle snapshot. No task transcripts or private answer manifests are included. A dated snapshot of all seven campaigns and the scoring/cause ledgers is also preserved in [history/2026-10-04](../history/2026-10-04/README.md).

| Campaign | Rows | Report | Results | Machine-readable report | Lifecycle |
|---|---:|---|---|---|---|
| `seed67-qwen38flash-gpt6luna-recovery-20261002` | 13 | [Markdown](runs/seed67-qwen38flash-gpt6luna-recovery-20261002/report.md) | [CSV](runs/seed67-qwen38flash-gpt6luna-recovery-20261002/results.csv) | [JSON](runs/seed67-qwen38flash-gpt6luna-recovery-20261002/report.json) | [JSON](runs/seed67-qwen38flash-gpt6luna-recovery-20261002/lifecycle.json) |
| `seed67-step1-six-models-3rep-3mcp-20260930` | 72 | [Markdown](runs/seed67-step1-six-models-3rep-3mcp-20260930/report.md) | [CSV](runs/seed67-step1-six-models-3rep-3mcp-20260930/results.csv) | [JSON](runs/seed67-step1-six-models-3rep-3mcp-20260930/report.json) | [JSON](runs/seed67-step1-six-models-3rep-3mcp-20260930/lifecycle.json) |
| `deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` | 4 | [Markdown](runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929/report.md) | [CSV](runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929/results.csv) | [JSON](runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929/report.json) | [JSON](runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929/lifecycle.json) |
| `luna-nous-shared-matrix-seed67-3mcp-20260929` | 8 | [Markdown](runs/luna-nous-shared-matrix-seed67-3mcp-20260929/report.md) | [CSV](runs/luna-nous-shared-matrix-seed67-3mcp-20260929/results.csv) | [JSON](runs/luna-nous-shared-matrix-seed67-3mcp-20260929/report.json) | [JSON](runs/luna-nous-shared-matrix-seed67-3mcp-20260929/lifecycle.json) |
| `glm53flash-shared-matrix-seed67-3mcp-20260929` | 4 | [Markdown](runs/glm53flash-shared-matrix-seed67-3mcp-20260929/report.md) | [CSV](runs/glm53flash-shared-matrix-seed67-3mcp-20260929/results.csv) | [JSON](runs/glm53flash-shared-matrix-seed67-3mcp-20260929/report.json) | [JSON](runs/glm53flash-shared-matrix-seed67-3mcp-20260929/lifecycle.json) |
| `shared-matrix-seed67-bloodhound-nous-codex-20260928` | 8 | [Markdown](runs/shared-matrix-seed67-bloodhound-nous-codex-20260928/report.md) | [CSV](runs/shared-matrix-seed67-bloodhound-nous-codex-20260928/results.csv) | [JSON](runs/shared-matrix-seed67-bloodhound-nous-codex-20260928/report.json) | [JSON](runs/shared-matrix-seed67-bloodhound-nous-codex-20260928/lifecycle.json) |
| `qwen3.8-json-rerun-2` | 5 | [Markdown](runs/qwen3.8-json-rerun-2/report.md) | [CSV](runs/qwen3.8-json-rerun-2/results.csv) | [JSON](runs/qwen3.8-json-rerun-2/report.json) | [JSON](runs/qwen3.8-json-rerun-2/lifecycle.json) |

## Reading the reports

All 21 cross-campaign comparisons fail the saved compatibility gate; do not pool their scores. The original three-pass campaign and its recovery have different scope. Missing cost values mean not recorded, not zero cost.

The report JSONs include question-level outcome and usage summaries, identifiers, and fingerprints, but no raw model/tool transcripts or reference-answer contents.

Generated labels such as “Publication status: not published” describe the source artifact at generation time; they do not describe the current visibility of this repository.

The model-card Markdown retains cohort and repetition details. Use those details with the images, rather than interpreting every row as a controlled comparison.
