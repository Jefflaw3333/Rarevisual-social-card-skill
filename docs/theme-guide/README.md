# Rare Visual Theme System — Documentation

This directory contains the **complete style guide** for the Rare Visual social card skill's 10-theme palette system. It is the single source of truth for brand colors, typography, content routing, and production rules.

## 📂 Files

| File | Language | Audience | Notes |
|------|----------|----------|-------|
| [`theme-guide-en.html`](./theme-guide-en.html) | English | International designers, overseas collaborators | Use for sharing with contractors and freelancers |
| [`theme-guide-zh.html`](./theme-guide-zh.html) | 中文 | 内部设计师 + 国内同事 | **Recommended default for Rare Visual team** — full Chinese localization |

Both files are **single-file HTML** with inline CSS — open in any modern browser. No build step, no dependencies, no fonts to install (Google Fonts load via CDN).

## 🎨 What's in the guide

Each file contains 6 sections:

1. **Editorial Magazine × E-ink** — 6 magazine-style themes (warm-brass / burnished-brass / stone-blue / olive-stone / ivory / midnight-brass) with live CSS preview cards
2. **Swiss International** — 4 Swiss-style accents (rv-gold / honey / sage / brick) with live CSS preview cards
3. **Usage guide** — 15-row scenario → recommended-theme lookup table with rationale
4. **Color tokens** — Complete CSS-variable reference for all 10 themes (paper / ink / accent hex + RGB values)
5. **Typography** — 9 real-size type samples (Editorial h-display 80px → Swiss h-hero 120px)
6. **Rules** — 12 hard rules and pitfalls (larger = lighter, one accent, never pure black/white, no AI purple, etc.)

## 🔧 How to use this guide

**For card generation**: when you (or your AI agent) generate a Rare Visual social card, refer to section 3 (usage guide) to pick the right theme for the content type, then copy the hex values from section 4 (color tokens).

**For review**: send `theme-guide-zh.html` to brand reviewers, designers, or stakeholders. The single-file HTML opens anywhere and prints cleanly to PDF.

**For onboarding**: when a new designer joins the Rare Visual team, share this guide as the first reference. It encodes the brand voice (`intentional, warm, grounded, discerning, effortless`) into concrete tokens and rules.

## 📐 Generation rules (summary)

The 12 hard rules in section 6 are non-negotiable. The most critical:

- **Larger = lighter**: big display text must use lower font weight (Editorial 500, Swiss 200-300)
- **One accent only**: never mix rv-gold + honey in one deck
- **Never pure black/white**: use `#faf6ee` (ivory) and `#1a1612` (warm near-black)
- **Default to `warm-brass`**: 80% of content fits the default theme

## 🔗 Related

- Skill source: <https://github.com/Jefflaw3333/Rarevisual-social-card-skill>
- Skill root: [`../SKILL.md`](../SKILL.md)
- Theme preset reference: [`../references/theme-presets.md`](../references/theme-presets.md)
- Layout recipes: [`../references/layout-recipes.md`](../references/layout-recipes.md)

---

**Fork lineage**: this guide is part of the Rare Visual fork of [guizang-social-card-skill](https://github.com/op7418/guizang-social-card-skill) v0.15 (AGPL-3.0). The HTML format, theme CSS variables, and 28 layout skeleton structure are inherited unchanged. Only the palette, theme names, copy vocabulary, and category routing have been retuned for Rare Visual.
