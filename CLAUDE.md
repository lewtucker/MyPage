# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Personal portfolio/about page for Lew Tucker, hosted on GitHub Pages. Pure static HTML — no build step, no dependencies, no framework.

## Structure

- `index.html` — the entire site, single self-contained file with inline CSS and JS

## Deployment

GitHub Pages serves `index.html` directly from the repo root. To deploy, push to the `main` branch (or whichever branch is configured as the Pages source in repo settings).

## Design constraints

- No external dependencies — all CSS and JS must be inline or in local files
- Light background, minimal/editorial aesthetic using Georgia serif for headings
- Color palette defined via CSS variables at the top of `<style>`: `--bg`, `--text`, `--muted`, `--accent`, `--rule`
- Accent color is warm terracotta (`#8b6f5e`)

## Layout & animation

- Single centered column, max-width 540px
- Headings use Georgia serif; labels and nav links use system sans-serif (`-apple-system, "Helvetica Neue", Arial`)
- `.rule` decorative divider: full-width 1px line with a short accent-colored segment on the left via `::after`
- Nav links are small-caps uppercase with underline that transitions to accent color on hover
