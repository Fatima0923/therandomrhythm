# therandomrhythm.com

Working repo for managing [therandomrhythm.com](https://therandomrhythm.com), a
WordPress + Elementor site, via the `the-random-rhythm-elementor` MCP server.

See [CLAUDE.md](CLAUDE.md) for the rules Claude follows when editing this site
(backups before edits, draft-first, no secrets in this repo).

## Layout

- `snapshot/` — baseline read-only export of the live site: every page's
  Elementor data plus the kit/global styles and site settings (see
  `snapshot/INDEX.md`). Tagged in git as a recovery point.
- `backups/` — per-edit Elementor data snapshots taken immediately before
  changing a page.
- `docs/` — site documentation, including `site-map.md`.
