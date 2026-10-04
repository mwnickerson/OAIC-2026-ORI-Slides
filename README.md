# Stop Giving Models Open-Book Tests

Matthew Nickerson · Offensive AI Con 2026 · Offensive Reasoning Index (ORI)

## Slides and talking points

- [Slides — 36-page PDF](slides/ori-oaic-2026.pdf)
- [Speaker-style talking-points outline](talking-points.md), following the slide order and the spoken script
- [References and cited result files](references/README.md)

## Results and model cards

The October 4, 2026 report snapshot covers **seven campaigns, 114 aggregate rows, and 37 model/route cards**.

- [Executive summary — PDF](reports/ori-recent-runs-2026-10-04/recent-runs-executive-summary.pdf) · [Markdown](reports/ori-recent-runs-2026-10-04/recent-runs-executive-summary.md)
- [Full analysis — PDF](reports/ori-recent-runs-2026-10-04/analysis.pdf) · [Markdown](reports/ori-recent-runs-2026-10-04/analysis.md) · [JSON](reports/ori-recent-runs-2026-10-04/analysis.json)
- [All model cards](reports/ori-recent-runs-2026-10-04/model-cards/README.md) — Markdown, SVG, and PNG for each pairing
- [Campaign reports and original CSV results](reports/README.md)
- [Dated run history and scoring/cause ledgers](history/README.md)

The current benchmark scope is **seed 67 only**; the planned three-seed expansion is cancelled. The existing three-pass results repeat the same 50 questions, not three environments or 150 unique questions. Earlier development scorecards in the talk remain historical context, not additional current-seed cohorts.

Keep each campaign's cohort, settings, repetition, and coverage with its score. These reports include interrupted runs, infrastructure failures, and unattempted slots; they are not a pooled leaderboard. Recovery runs are separate results, and unattempted work is not measured zero capability.

This repository contains the slide PDF, talking points, reports, model cards, and references—not private rehearsal notes, raw conversations, or production scripts. Machine-specific source paths were shortened in the analysis Markdown and JSON; the original per-run reports, CSVs, and model cards are unchanged.

## How to read the results

Right + wrong = scored. Scored + unscored = scheduled. Attempted requests, retries, provider/tool events, campaign lifecycle and teardown are separate. The corrected [question ledger](reports/ori-recent-runs-2026-10-04/question-scoring-ledger.json) and [presentation-status ledger](reports/ori-recent-runs-2026-10-04/presentation-status-ledger.json) keep these distinctions explicit; cleanup does not invalidate recorded answers. The [seed explanation](references/data/ref-12-seed-mechanics.md) separates generated environments from task compilation and model randomness.
