# Just the Games

Fast, interactive reference for running tabletop RPGs in the browser. Built on [Just the Docs](https://github.com/just-the-docs/just-the-docs) with plugins for dice, link previews, clickable maps, and more.

**Live site:** [games.puzzledungeon.com](https://games.puzzledungeon.com)

## What's here

- **[Old-School Essentials rules](docs/ose-rules.md)** — SRD reference (from the [Obsidian TTRPG Community markdown](https://github.com/Obsidian-TTRPG-Community/Old-School-Essentials-Markdown))
- **Adventures** — [Puzzle Dungeon: The Seers Sanctum](docs/seers-sanctum.md), [A Familiar Tower](docs/a-familiar-tower.md)
- **[Make Your Own](docs/make-your-own.md)** — creator guides, plugin overview, and an adventure template

## Features

| Feature | What it does |
| --- | --- |
| Dice tray | Click dice notation (`3d6`, `2-in-6`, etc.) or random tables to roll |
| Hover previews | Preview internal links; pin, move, and resize windows |
| Image maps | Clickable regions on maps and dungeon layouts |
| TOC in nav | Document headings appear in the sidebar |
| RPG callouts | Extra callout styles for adventure text |
| Dark theme | Dark overlay on the default Just the Docs look |

These plugins work on any Just the Docs site. See the [plugin overview](docs/make-your-own/plugin-feature-overview.md), or start from the [Just the Games template](https://github.com/sunflowermans/just-the-games-template).

## Local development

Requires [Ruby](https://www.ruby-lang.org/), [Bundler](https://bundler.io), and [Jekyll](https://jekyllrb.com).

```bash
bundle install
bundle exec jekyll serve
```

Preview at [localhost:4000](http://localhost:4000). The built site is written to `_site/`.

For faster local builds, you can temporarily exclude large rule trees in `_config.yml` (see the commented `exclude` example there).

## Deploy

Pushes to `main` build and publish via GitHub Actions (`.github/workflows/jekyll.yml`) to GitHub Pages. Site URL is set in `_config.yml`.

## License

- Site theme/template heritage: [MIT](LICENSE) (from Just the Docs)
- OSE rules content: Open Game License (see [docs/ose-rules/license.md](docs/ose-rules/license.md))
- Adventures on this site: see each adventure’s own license notice (typically CC BY-NC for text; artwork remains the artists’)

Fonts, colors, and styles are based on the [Designing Dungeons](https://dungeons.hismajestytheworm.games/) course and used with permission.
