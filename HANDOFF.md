# HANDOFF

Updated 2026-11-20 (demo panel alignment).

## Done
- Community files (2026-11-24, Chase: will engineers see an amateur repo): added CONTRIBUTING, CODE_OF_CONDUCT, issue templates and a PR template (plus SECURITY.md where missing), per `studio-agents` docs/repo-standards.md. Next: set the repo description and topics in GitHub settings, add a CI badge.
- Library (`hero-backgrounds.js`), self-contained demo (`index.html`), MIT license, README published to `main`.
- Checked: no dependencies, no third-party hosts, no fonts loaded from outside.
- Demo served from GitHub Pages. Workflow `.github/workflows/pages.yml` deploys `index.html` and `hero-backgrounds.js` on every push to `main` (Pages source must be set to GitHub Actions).

## In progress
- PR: title stays clear of the settings panel; line colour now fades the accent toward the page colour, so greyscale accents no longer change line strength and dark pages stay visible. Waiting on Chase to merge; merging deploys to Pages.

## Next step
- Chase: review and merge the demo PR, then send the Pages URL to the site thread so chaseholroyd.com can link it.
- Chase: Settings, Pages, Source = GitHub Actions (after the workflow PR merges).
- Add a row for this repo to the pm-tools board (BOARD.md) in a small PR.
- LinkedIn post (owned by the Role Radar project).

## Decisions to review
- Demo is `index.html` with the library inlined so it works as a single file. Edit `hero-backgrounds.js` and re-inline if the library changes.

## Blockers
- None.

## Repo best-practices pass (2026-11-25)
- Done: added `.github/CODEOWNERS`, weekly Actions Dependabot and a `.gitignore`. Part of the GitHub best-practices audit; see studio-agents docs/repo-standards.md.
