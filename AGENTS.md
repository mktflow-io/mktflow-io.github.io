# AGENTS.md

Guidance for AI coding agents working in this repository.

## Overview

This repo hosts the **static landing page** for the mktflow-io organization, published via
GitHub Pages at https://mktflow-io.github.io.

## Repository Contents

| Path | Purpose |
|------|---------|
| `index.html` | Single-page landing (self-contained HTML + inline CSS, no build step) |
| `assets/logo.png` | Organization logo (Ukiyo-e style, ~850 KB) |

## Conventions

- **Pure static, no build system.** `index.html` is self-contained — edit it directly and push to
  `main` to publish. No npm, no framework, no CI.
- **Logo is the canonical copy** referenced elsewhere by URL
  (`https://mktflow-io.github.io/assets/logo.png`, e.g. the `mktflow-io/.github` profile README).
  Keep it here; do not remove or rename without updating those references.
- **Brand colors** used in `index.html`: background `#0a1628` (navy), accent `#c8a84e` (gold).
  Stay consistent with these.
- **Commit language**: French (matches existing history).

## Editing

Edit `index.html` or `assets/`, commit to `main`. GitHub Pages deploys automatically from the
default branch.

---

| Property | Value |
|----------|-------|
| **Repo** | `mktflow-io/mktflow-io.github.io` |
| **URL** | https://mktflow-io.github.io |
| **Last updated** | 2026-08-14 |
