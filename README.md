# ALIR 2026 — Zammermoos Time-Owed Board

Handicap reference for the navigator of **Zammermoos** (Club Swan 42, Uni 4224, PHRF -15, Spinnaker Div 9) in the 49th Around Long Island Regatta, July 23-26 2026.

**Live:** https://zammermoos.github.io/alir-2026/

Single-file static app (`index.html`), no build step, no dependencies.

## What it shows

For every boat in the fleet, the corrected-time margin vs Zammermoos expressed in **finish-line clock time** — start staggers between divisions are folded in, so green means they can cross ahead of us by anything *less* than the margin and we still win on corrected; red means we must cross *more* than the margin ahead of them. A gap of exactly the margin is a corrected-time dead heat.

- Margin = (our start - their start) + (our rating x our distance - their rating x their distance)
- Scoring per 2026 ALIR SIs v1.0: PHRF time-on-distance, YRA of LIS distance-race ratings, 207 nm (Around Long Island) / 230 nm (Around the Islands)
- Tap a boat for a head-to-head panel with a finish-time deadline calculator
- Start times, course distances, race date, and ratings are editable for postponements and scratch-sheet amendments; only edited values persist (localStorage), so an updated scratch sheet is never shadowed by stale saves
- ORC Division 0 is scored under ORC APH — not comparable to PHRF, listed for reference only

## Updating the scratch sheet

Edit the `DIVISIONS` and `BOATS` arrays in `index.html` and push to `main`; GitHub Pages redeploys automatically.
