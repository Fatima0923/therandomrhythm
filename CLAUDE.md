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

- `snapshot/` — the baseline, read-only export of the live site (every page's
  Elementor data, the kit/global styles, and site settings), tagged in git as
  a recovery point. Not updated on every edit — see `backups/` for that.
- `backups/` — per-edit Elementor data snapshots taken immediately before
  changing a page (see rule 1 above).
- `docs/` — site documentation (e.g. `site-map.md` listing current pages).
