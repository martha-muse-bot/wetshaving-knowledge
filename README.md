# Wetshaving Knowledge

A human- and agent-readable Obsidian vault of community history and
learnings from the r/Wetshaving shave-of-the-day world: brand lineages,
renames, closures and collaborations; hardware lore; product aliases and
naming traps; product lines and bases; the people behind the makers;
community shorthand; and the open questions still being worked.

## Read it

- **Browse the site:** https://martha-muse-bot.github.io/wetshaving-knowledge/
- **Open as an Obsidian vault:** clone this repo and open the repo root
  in Obsidian. Notes live under `content/` and link to each other with
  `[[wikilinks]]`; the graph view shows how makers, products, and people
  connect.

## How a note is organized

Every note carries frontmatter with its source file, a confidence level,
and a learned date when one is recorded:

- **established** — confirmed by a primary or strong source
- **lead** — plausible but only partly verified; treat names as pointers
- **unknown** — no confidence statement recorded in the source entry

Section indexes (`content/*/index.md`) list every note in that section,
and `content/index.md` is the vault home.

## Scope note

This vault is a snapshot of the community knowledge base as of 2026-10-28.
Solved backlog items are not listed under Open questions: their findings
already live in the main notes. The working run record (learning log) is
not published here. The underlying SOTD dataset and canonical product
catalog are separate projects; this vault is the human-readable history.

## Build it yourself

Quartz v5. Requires Node.js v22+ and npm 10.9.2+.

```bash
npm ci
npx quartz build        # output in public/
npx quartz build --serve  # local preview
```

The site deploys to GitHub Pages automatically on every push to `main`
via `.github/workflows/deploy.yml`.

## License

Quartz itself is MIT-licensed (see `LICENSE.txt`). The vault content is
community history compiled from public sources; sources are cited in the
notes themselves.
