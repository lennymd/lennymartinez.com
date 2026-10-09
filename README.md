# Lenny Martinez's Website

Code for my website.

Built with [Hugo](https://gohugo.io/) (v0.167.0, matching the Netlify build env) and deployed on Netlify via `hugo --gc --minify`.

## Setup

```sh
npm install   # dev dependencies only — Hugo itself is installed separately
hugo server   # local preview at http://localhost:1313
```

### Packages

Both are dev-only; nothing is bundled into the site.

- **prettier** — formats the Markdown in `content/`, `assets/css/main.css`, and the JSON config files. Note that Prettier has no TOML parser, so `hugo.toml` is formatted by hand.
- **prettier-plugin-go-template** — parses Hugo template syntax so the `.html` files in `layouts/` aren't mangled by the standard HTML parser.

Config lives in `.prettierrc`: 2-space indent, 80-column width, LF endings. The `overrides` block routes `*.html` through the `go-template` parser. The JS-specific options (`semi`, `singleQuote`, `trailingComma`, `arrowParens`, `bracketSpacing`) are carryover defaults — the site has no JS.

Run it with `npx prettier --write .`.

### .markdownlint.json

Rule overrides for markdownlint. Three defaults are disabled:

- `MD034` (bare URLs) — plain URLs are fine in content and in this README.
- `MD013` (line length) — prose isn't hard-wrapped; formatting is left to the editor.
- `MD033` (inline HTML) — Hugo content mixes in HTML and shortcodes.

## Adding content

Each section has an archetype in `archetypes/` that pre-fills the front matter. New files start as drafts: set `draft = false` to publish, or preview drafts with `hugo server -D`.

```sh
hugo new news/2026-10-09-short-slug.md       # news update: date + a sentence or two of Markdown
hugo new publications/my-paper-name.md       # publication: title, venue, description, head image
hugo new projects/my-project-name.md         # work project: title, subtitle, description, head image
```

- **News** items have no page of their own; they're listed on `/news/` and the latest 3 show on the home page. Prefix filenames with the date so they sort in order.
- **Publications** use `venue` for the line under the title, e.g. `'CHI 2025'` or `'Under review'`.
- **Projects** use `subtitle` for that line, e.g. `'design fiction, 2023'`.

Lists are sorted by `date`, so set it to when the thing happened, not when the file was created.

## Favicons

Favicon assets live in `static/favicon/` and are generated at <https://favicon.io/svg-favicon/>. To update, modify the `static/favicon/lennymartinez.svg`, regenerate the set there and replace:

- `static/favicon.ico` — legacy fallback
- `static/favicon/apple-touch-icon.png`
- `static/favicon/android-chrome-192x192.png` and `-512x512.png` (referenced from the web manifest)

These are wired up in `layouts/_partials/head.html`, alongside the manifest generated from `assets/manifest.json`.

## FUTURE TASKs

- [ ] add speculating AI summer school project
- [ ] add news21 project
- [ ] create **gallery section** for photos
- [ ] create **notes section** for mini-blog.
- [ ] Update **render-image** to use srcset
- [ ] Implement **JSON-LD `Person` schema.**
