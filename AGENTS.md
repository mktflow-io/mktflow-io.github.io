# AGENTS.md

Guidance for AI coding agents working in this repository.

## Overview

This repo hosts the **static landing page** for the mktflow-io organization, published via
GitHub Pages at https://mktflow-io.github.io.

## Where the repository lives

Since 2026-10-11 the repository is hosted on the Daftech forge: https://git.daftech.io/mktflow-io/mktflow-io.github.io
(tickets and pull requests there; `main` is protected, merges by the user only).
https://github.com/mktflow-io/mktflow-io.github.io is a read-only push mirror, kept because GitHub Pages still
publishes the site from it until phase 6 of the migration (daftech-cluster, `docs/forge/CONCEPTION.md` § 4.1,
decision 30). GitHub Actions is disabled on the mirror: `.nojekyll` makes Pages serve the files as they are.

## Repository Contents

| Path | Purpose |
|------|---------|
| `index.html` | Single-page landing (self-contained HTML + inline CSS, no build step) |
| `assets/logo.png` | Organization logo (Ukiyo-e style, ~850 KB) |
| `.nojekyll` | Empty; GitHub Pages publishes the files without a Jekyll build (needed with Actions disabled) |

## Conventions

- **Pure static, no build system.** `index.html` is self-contained — open a pull request on the forge;
  once merged, the push mirror carries `main` to GitHub and Pages publishes it. No npm, no framework, no CI.
- **Logo is the canonical copy** referenced elsewhere by URL
  (`https://mktflow-io.github.io/assets/logo.png`, e.g. the `mktflow-io/.github` profile README).
  Keep it here; do not remove or rename without updating those references.
- **Brand colors** used in `index.html`: background `#0a1628` (navy), accent `#c8a84e` (gold).
  Stay consistent with these.
- **Commit language**: French (matches existing history).

## Editing

Edit `index.html` or `assets/` in a branch, open a pull request on the forge, get it merged. GitHub Pages
deploys automatically from the mirrored default branch (check: `gh api repos/mktflow-io/mktflow-io.github.io/pages/builds/latest`).

---

| Property | Value |
|----------|-------|
| **Repo** | https://git.daftech.io/mktflow-io/mktflow-io.github.io (mirror: `mktflow-io/mktflow-io.github.io` on GitHub) |
| **URL** | https://mktflow-io.github.io |
| **Last updated** | 2026-10-11 |
