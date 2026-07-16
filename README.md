# The Almanac — Test Tracker

Public validation tracker for **The Almanac: Trades, Callings & Mastery**, the trade-progression
mod running on **The Quire** (a whitelisted Vintage Story server). The mod source is private; this
repo holds only the beta test workflow.

## How it works

1. The **testing board** on the Quire site lists what needs validating, drawn from the mod's
   validation doc. Each card is one test item (a verb, an axis, a specific behaviour).
2. Pick an item and hit **Test this**. It opens a prefilled [test report](../../issues/new?template=test-report.yml)
   here on GitHub — the item and the ask are already filled in.
3. Run it in-game, fill in what happened, and submit. Your report is a GitHub issue.
4. A maintainer reviews it: **approved**, or **changes-requested** with a comment asking for more.

Think of a report like a pull request — you submit evidence that a thing works, and it gets
reviewed before it counts as validated.

## Labels (the board columns)

| Label | Meaning |
|-------|---------|
| `needs-review` | A fresh submission awaiting a maintainer. |
| `changes-requested` | Maintainer needs more (a repro, a screenshot, a retest). |
| `approved` | Validated. The item is proven. |
| `blocked` | Can't be tested yet (missing dependency, server state). |
| domain tags (`WOO`, `MIN`, `MET`, …) | Which trade the item belongs to. |

## Who can submit

Testers on The Quire whitelist. Anyone can read; the board gates submission behind your VS
username. Reports are tied to your GitHub account for accountability.
