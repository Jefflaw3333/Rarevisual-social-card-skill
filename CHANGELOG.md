# Changelog

All notable changes to `rarevisual-social-card-skill` are documented here. This fork is a brand retune of upstream [guizang-social-card-skill](https://github.com/op7418/guizang-social-card-skill) — visual workflow, 28 layout skeletons, 9-rule validator, and production pipeline are inherited unchanged.

## 1.0.0-rv.1 — 2026-07-09 — Rare Visual fork initial release

### Added
- **Rare Visual palette** in `references/theme-presets.md`:
  - 6 Editorial themes: `warm-brass` (default), `burnished-brass`, `stone-blue`, `olive-stone`, `ivory`, `midnight-brass`
  - 4 Swiss accents: `rv-gold` (default), `honey`, `sage`, `brick`
- **RV brand context** in SKILL.md, README.md, README.en.md, agents/openai.yaml, package.json
- **Migration sed script** in `references/theme-presets.md` for renaming legacy local-tests
- **Brand lift rationale** per theme: which RV content types each theme fits best

### Changed
- `assets/template-editorial-card.html` — 6 new theme blocks replacing the upstream Guizang themes
- `assets/template-swiss-card.html` — 4 new accent blocks replacing IKB Blue / Lemon / Safety Orange
- `SKILL.md` — frontmatter `name` set to `rarevisual-social-card-skill`; description tuned to RV triggers; theme switching lines updated
- `README.md` and `README.en.md` — headers rewritten to RV fork context; default themes called out
- `package.json` — `name`, `version`, `description`, `keywords`, `author`, `license` updated
- `agents/openai.yaml` — `display_name`, `brand_color`, `default_prompt` updated to RV brand

### Inherited unchanged
- 28 layout skeletons (M01-M16 Editorial, S01-S12 Swiss) in `references/layout-recipes.md`
- 9-rule Playwright validator (`validate-social-deck.mjs`)
- Component class system (`references/components.md`, font stacks, type scale, weight mapping)
- 3-canvas size system (`.poster.xhs` 1080×1440, `.poster.square` 1080×1080, `.poster.wide` 2100×900)
- Pair-preview frame system
- Lucide icon rule (Swiss), Noto Serif / Sans / Playfair / IBM Plex Mono (Editorial)
- Live Photo production rules (`references/live-photo-production.md`)
- WebGL magazine background (`assets/magazine-bg-webgl.js`)
- Screenshot background WebP assets (`assets/screenshot-backgrounds/`)

### License
- AGPL-3.0 retained from upstream. See `LICENSE`.
- All derivatives must remain open-source under AGPL-3.0 or compatible license.
- "Network use is distribution" applies: any SaaS / web service running this skill must publish source.

### Fork lineage
- Upstream: `op7418/guizang-social-card-skill` v0.15 (commit `cf4b810` — "docs: expand Live Photo README guide")
- Branch: `rv-rebrand`
- This fork: `Jefflaw3333/Rarevisual-social-card-skill`