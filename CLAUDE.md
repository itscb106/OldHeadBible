# Old Head Fantasy Holy Bible — site repo

This repo is the served website (GitHub Pages, branch `main`, case-sensitive URL
`https://itscb106.github.io/OldHeadBible/`). `index.html` is the whole app, standalone.

## Governing principles for all site content
1. **Every number, name, record, and injury shown on this site is computed or pulled
   from source (the league's ESPN data) at build time — never typed in by hand or
   recalled from memory.** The page renders generated data (`const SD`, `const PROF`).
   Don't hand-edit a stat into the HTML; fix it in the data pipeline and regenerate.
2. **One truth, everywhere.** The same fact appears across many tabs (and in the
   project's podcast and memory). A change in one place must be reflected in all of
   them — so fix the source data and regenerate, rather than editing one surface out
   of sync with the rest.

The site rebuilds **every Tuesday morning** from a fresh data pull — all tabs at once,
along with the rest of the project — so they always agree.

## Rules when editing this site
- **Clinched / Eliminated are deterministic** (a true playoff-feasibility result),
  never odds thresholds. An alive sub-1% team shows `<1%`, not "Eliminated."
- **AI-written content ("✍️ The Word") is additive** — it layers on top of existing
  content; it never removes a trophy case, chart, haul, or stat.
- **Honest timestamps stay honest** — the "Stats thru Wk N" stamps and footer
  sourcing note must reflect the actual last build.
- **Mobile and desktop both** — verify no element overflows the viewport and every
  nav tab is reachable at phone width before shipping a layout change.
- **Keep it unlisted** (`noindex,nofollow` + robots Disallow).

The full content rulebook and the weekly build pipeline live in the private project
repo, not here.
