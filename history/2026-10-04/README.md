# 2026-10-04 — ORI report and run archive

This is a dated snapshot of seven historical campaigns run September 28–October 3, 2026. It records 114 model/track/repetition rows and preserves the per-run source reports alongside the corrected public scoring and presentation-status ledgers.

## Archive contents

- [`question-scoring-ledger.json`](question-scoring-ledger.json) — one row per model/track/repetition result, including right/wrong/scored counts, scheduled and unscored coverage, public outcome causes, and usage fields.
- [`presentation-status-ledger.json`](presentation-status-ledger.json) — reason-specific labels derived from scored coverage and public outcome causes.
- [`runs/`](runs/) — byte-for-byte snapshot copies of the seven public run folders already linked from [`reports/README.md`](../../reports/README.md). Each folder retains its report Markdown, report JSON, aggregate CSV, and lifecycle JSON; the original paths remain available for compatibility.
- [Current analysis](../../reports/ori-recent-runs-2026-10-04/analysis.md), [executive report](../../reports/ori-recent-runs-2026-10-04/recent-runs-executive-summary.md), and [model cards](../../reports/ori-recent-runs-2026-10-04/model-cards/README.md).

## Aggregate coverage

| Measure | Total |
|---|---:|
| Right | 2,299 |
| Wrong | 783 |
| Scored | 3,082 |
| Scheduled | 5,700 |
| Attempted | 3,635 |
| Unscored | 2,618 |

The 114 rows span different campaigns and repetitions. These sums describe workload and coverage; they are not a pooled accuracy denominator. Direct and MCP results remain separate, and none of the 21 cross-campaign compatibility comparisons passed the saved gate.

Unscored outcome totals: `MISSING` 2,065; `OUTPUT_INVALID` 324; `INFRA_ERROR` 73; `QUERY_ERROR` 66; `TASK_TIMEOUT` 76; `QUERY_TIMEOUT` 13; `INTERRUPTED` 1. These outcome codes explain unscored coverage where the public reports support attribution; retry/error event tallies are kept separate from unique-question counts.

A row-by-row comparison against the preceding Slides-repo analysis found no changes in right, wrong, scored, scheduled, unscored, cause, or presentation-status values across the 114 matching result keys. The refreshed report wording preserves operational and teardown caveats instead of treating them as reasoning outcomes.

## Provenance and privacy

The source bundle was read-only retrieved and its hash/member inventory verified against the NAS. The existing per-run report files are preserved without transformation in this archive. The raw source `analysis.json` and original ZIP are not duplicated here; the repository's existing path-sanitized analysis JSON remains the public copy. No raw prompts, private answer contents, model/tool transcripts, or credentials are included. Per-run public JSONs may retain identifiers and fingerprints, as documented in [`reports/README.md`](../../reports/README.md).

The source supplied the same HTML and PDF bytes for the analysis and executive-report names; the repository keeps distinct rendered derivatives for those names. The Markdown reports remain separate.
