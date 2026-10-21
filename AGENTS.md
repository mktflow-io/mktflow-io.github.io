# AGENTS.md

Guidance for AI coding agents working in this repository.

## Overview

This repo hosts the **static landing page** for the mktflow-io organization, published via
GitHub Pages at https://mktflow-io.github.io.

## Where the repository lives

Since 2026-10-11 the repository is hosted on the Daftech forge: https://git.daftech.io/mktflow-io/mktflow-io.github.io
(tickets and pull requests there; `main` is protected, merges by the user only).
https://github.com/mktflow-io/mktflow-io.github.io is the copy GitHub Pages publishes from. It no longer follows the
forge: its push mirror was removed when the mirror closed (phase 6 of the migration, 2026-10-22, daftech-cluster,
`docs/forge/CONCEPTION.md` § 4.1), and it is archived, read-only, since that day. GitHub Pages still serves the page
from the archived copy (checked at the archiving). GitHub Actions is disabled on it, and **GitHub Pages does not
republish without Actions** (verified on 2026-10-11: `.nojekyll` does not change that). The published site stays
frozen at the content of commit `d1c29e6` until the page moves to the relay (decision 30). An urgent publication
before then means unarchiving the GitHub copy, updating it by hand, re-enabling Actions for one build, then disabling
Actions and archiving the copy again: ask the Coordinator first.

## Repository Contents

| Path | Purpose |
|------|---------|
| `index.html` | Single-page landing (self-contained HTML + inline CSS, no build step) |
| `assets/logo.png` | Organization logo (Ukiyo-e style, ~850 KB) |
| `.nojekyll` | Empty; tells GitHub Pages to skip the Jekyll build (it does not let Pages publish with Actions disabled) |

## Conventions

- **Pure static, no build system.** `index.html` is self-contained — open a pull request on the forge;
  once merged, nothing reaches GitHub any more (push mirror removed), so the published page does not change
  (see above). No npm, no framework, no CI.
- **Logo is the canonical copy** referenced elsewhere by URL
  (`https://mktflow-io.github.io/assets/logo.png`, e.g. the `mktflow-io/.github` profile README).
  Keep it here; do not remove or rename without updating those references.
- **Brand colors** used in `index.html`: background `#0a1628` (navy), accent `#c8a84e` (gold).
  Stay consistent with these.
- **Commit language**: French (matches existing history).

## Editing

Edit `index.html` or `assets/` in a branch, open a pull request on the forge, get it merged. The published site
does not follow until the page moves to the relay (see "Where the repository lives").

---

| Property | Value |
|----------|-------|
| **Repo** | https://git.daftech.io/mktflow-io/mktflow-io.github.io (archived copy on GitHub, which Pages publishes: `mktflow-io/mktflow-io.github.io`) |
| **URL** | https://mktflow-io.github.io |
| **Last updated** | 2026-10-21 |
