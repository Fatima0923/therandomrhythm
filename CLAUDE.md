# therandomrhythm.com

This repo manages content and design for **therandomrhythm.com**, a WordPress
site built with Elementor. Changes are made through the `the-random-rhythm-elementor`
MCP server (and related WordPress MCP tools), not by editing files that get
deployed directly — this repo is for backups, documentation, and working notes.

## Rules

1. **Back up before editing.** Before modifying a page's Elementor data, fetch
   its current data and save it to `backups/` (e.g.
   `backups/<page-slug-or-id>-<YYYY-MM-DD>.json`) before making any changes.
   This is the only way to recover a page if an edit goes wrong.

2. **Prefer drafts.** When creating or editing content, prefer saving as a
   draft rather than publishing directly. Only publish when the user
   explicitly asks for the change to go live.

3. **Never store secrets.** Never put passwords, API keys, auth tokens, or
   auth headers in any file in this repo (including backups, docs, or
   commit messages). Credentials belong in the MCP server's own
   configuration, not in this repository.

## Layout

- `backups/` — Elementor data snapshots taken before edits.
- `docs/` — site documentation (e.g. `site-map.md` listing current pages).
