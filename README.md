# Stop Giving Models Open-Book Tests

Matthew Nickerson · Offensive AI Con 2026 · Offensive Reasoning Index (ORI)

## Slides and talking points

- [Slides — 32-page PDF](slides/ori-oaic-2026.pdf)
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

The post-demo results sequence is: Early local scorecards → Different tests → Final three-run benchmark → Token usage → API rejections.

The [final scorecard and token breakdown](references/data/ref-13-final-benchmark.md) use an explicit per-repetition selection. GPT-6 Luna / Steven is **147/150**, from 50, 48 and 49 correct; its affected third repetition is replaced wholesale by the full rerun. Remaining coverage gaps belong to their own model/route rows. Native campaign reports and historical model cards remain available below as supporting records, not the talk’s final selected scorecard.

This repository contains the slide PDF, talking points, reports, model cards, and references—not private rehearsal notes, raw conversations, or production scripts. Machine-specific source paths were shortened in the analysis Markdown and JSON; the original per-run reports, CSVs, and model cards are unchanged.

## How to read the results

Right + wrong = scored. Scored + unscored = scheduled. Attempted requests, retries, provider/tool events, campaign lifecycle and teardown are separate. The corrected [question ledger](reports/ori-recent-runs-2026-10-04/question-scoring-ledger.json) and [presentation-status ledger](reports/ori-recent-runs-2026-10-04/presentation-status-ledger.json) keep these distinctions explicit; cleanup does not invalidate recorded answers. The [seed explanation](references/data/ref-12-seed-mechanics.md) separates generated environments from task compilation and model randomness.
