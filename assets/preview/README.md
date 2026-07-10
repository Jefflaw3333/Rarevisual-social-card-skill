# Theme Preview Cards

10 lightweight SVG mock cards — one per theme — that visually demonstrate the Rare Visual style system.

- Render natively in GitHub README (no Playwright, no build step)
- Look correct at any zoom level (SVG vector)
- Lightweight: total ~15 KB for all 10 cards
- Colors and typography match the production seed templates exactly

## Files

### Editorial (6 cards · 3:4 ratio 540×720)

| File | Theme | Best for |
|---|---|---|
| `warm-brass.svg` | Warm Brass (default) | Product photography, gifting covers |
| `burnished-brass.svg` | Burnished Brass | Collection launches, deeper tone |
| `stone-blue.svg` | Stone Blue | Material education, FAQ, comparison |
| `olive-stone.svg` | Olive Stone | Nature, semi-precious stones |
| `ivory.svg` | Ivory | Clean ecommerce product grids |
| `midnight-brass.svg` | Midnight Brass (dark) | Velvet, candle-lit, dark imagery |

### Swiss (4 cards · 16:9 ratio 720×405)

| File | Accent | Best for |
|---|---|---|
| `rv-gold.svg` | RV Gold (default) | Gift guides, FAQ, reviews |
| `honey.svg` | Honey | Q4 gifting, holiday countdowns |
| `sage.svg` | Sage | Eco, semi-precious, spring drops |
| `brick.svg` | Brick | Limited stock, urgent gifting |

## Notes

These are **hand-coded SVG mockups**, not screenshots. They match the production CSS variable definitions in `assets/template-editorial-card.html` and `assets/template-swiss-card.html`. The SVG uses system-font fallback names (serif, sans-serif, monospace) so GitHub's image renderer will use platform defaults — but the layout, hierarchy, and color are production-accurate.

For the full HTML version with real web fonts, see [`docs/theme-guide/`](../../docs/theme-guide/).
