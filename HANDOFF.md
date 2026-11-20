# HANDOFF

Updated 2026-11-20.

## Done
- Library (`hero-backgrounds.js`), self-contained demo (`index.html`), MIT license, README published to `main`.
- Checked: no dependencies, no third-party hosts, no fonts loaded from outside.
- Demo served from GitHub Pages. Workflow `.github/workflows/pages.yml` deploys `index.html` and `hero-backgrounds.js` on every push to `main` (Pages source must be set to GitHub Actions).

## In progress
- Nothing.

## Next step
- Chase: Settings, Pages, Source = GitHub Actions (after the workflow PR merges).
- Add a row for this repo to the pm-tools board (BOARD.md) in a small PR.
- LinkedIn post (owned by the Role Radar project).

## Decisions to review
- Demo is `index.html` with the library inlined so it works as a single file. Edit `hero-backgrounds.js` and re-inline if the library changes.

## Blockers
- None.
