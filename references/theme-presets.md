# Rare Visual Theme Presets

> Fork of `guizang-social-card-skill` v0.15, rebranded for **Rare Visual** (rarevisual.com) brand voice — *"Handcrafted accessories that turn everyday outfits into something intentional."*

Use **one theme for one image package**. Do not mix palettes across pages unless the user explicitly asks for a deliberate multi-chapter system.

All palettes are tuned for Rare Visual's brand personality: **intentional, warm, grounded, discerning, effortless**. Materials reference gold-filled, solid brass, semi-precious stones, and genuine leather. The accent colors are restrained and warm — never loud neon, never AI-purple, never chrome-bling.

---

## Editorial Magazine × E-ink Palettes (6 themes)

Adapted from Guizang's editorial mode for Rare Visual storytelling covers — product close-ups, gift guides, behind-the-scenes craftsmanship, and style essays.

### Warm Brass *(default — the Rare Visual signature)*

Use for product photography, gold-filled and brass close-ups, gifting covers, founder essays, and any post whose hero image is a piece of jewelry or a hand-crafted object on a warm neutral surface. This is the palette to reach for when in doubt.

```css
[data-theme="warm-brass"] {
  --paper:     #f5efe4;
  --paper-2:   #ebe1cf;
  --ink:       #2a2018;
  --muted:     #7a6a58;
  --line:      rgba(42,32,24,.22);
  --accent:    #b8924a;     /* RV gold — solid brass tone */
  --accent-soft: #d9c19a;
  --ink-rgb: 42,32,24;
  --paper-rgb: 245,239,228;
  --accent-rgb: 184,146,74;
}
```

**Why this works for RV:** warm cream paper evokes unboxing and product photography; the brass accent is unmistakably jewelry-language without being heavy. Pair with cream-paper backgrounds, hand shots, and natural-light photography.

---

### Burnished Brass *(deeper, more saturated)*

Use for hero covers that need more drama — collection launch announcements, "best of" gift roundups, and posts where the imagery has rich, saturated tones (gold-filled layered necklaces, brass-and-stone pairings).

```css
[data-theme="burnished-brass"] {
  --paper:     #ece1c8;
  --paper-2:   #ddcfb0;
  --ink:       #1f1610;
  --muted:     #6c5a44;
  --line:      rgba(31,22,16,.24);
  --accent:    #8f6a2e;     /* deeper brass — patina-aged */
  --accent-soft: #c7a87a;
  --ink-rgb: 31,22,16;
  --paper-rgb: 236,225,200;
  --accent-rgb: 143,106,46;
}
```

**Why this works for RV:** creates a richer, more antique-paper feel. Good when the imagery has warm wood, deep gold, or tan-leather tones. Avoid with bright pastel photography — the muted palette will fight it.

---

### Stone Blue *(calm analytical)*

Use for material education ("gold-filled vs plated" explainers), behind-the-scenes process posts, founder notes on quality/craftsmanship, and any piece that benefits from a cooler, less romantic palette.

```css
[data-theme="stone-blue"] {
  --paper:     #f2f4f5;
  --paper-2:   #e5ebef;
  --ink:       #0e1f33;
  --muted:     #5f6d78;
  --line:      rgba(14,31,51,.20);
  --accent:    #315d93;
  --accent-soft: #d7e1ec;
  --ink-rgb: 14,31,51;
  --paper-rgb: 242,244,245;
  --accent-rgb: 49,93,147;
}
```

**Why this works for RV:** the cool counterpoint to warm-brass. Use when the post needs credibility and clarity (quality education, FAQ, comparison posts). Pairs well with crisp product line-ups, swatch boards, and clean studio photography.

---

### Olive Stone *(grounded natural)*

Use for outdoor and travel posts ("packing jewelry for a trip"), nature photography, sustainability messaging, behind-the-scenes at markets or photoshoots, and grounded lifestyle content.

```css
[data-theme="olive-stone"] {
  --paper:     #f1ede0;
  --paper-2:   #e3dccc;
  --ink:       #1f2a1a;
  --muted:     #5d665d;
  --line:      rgba(31,42,26,.22);
  --accent:    #6b7f4a;     /* muted olive — semi-precious stone */
  --accent-soft: #c8d2b5;
  --ink-rgb: 31,42,26;
  --paper-rgb: 241,237,224;
  --accent-rgb: 107,127,74;
}
```

**Why this works for RV:** semi-precious stone colors (moss agate, jade, labradorite) sit naturally on this palette. Use when the imagery leans into nature, natural materials, or slow-paced brand-storytelling.

---

### Ivory *(clean commercial)*

Use for gift roundups, "shop the look" posts, clean product line-ups, customer testimonial spotlights, and any post where the imagery is the star and the design should disappear.

```css
[data-theme="ivory"] {
  --paper:     #faf6ee;
  --paper-2:   #f0e9da;
  --ink:       #1a1612;
  --muted:     #80766a;
  --line:      rgba(26,22,18,.20);
  --accent:    #c3a263;     /* softer brass — sand-blasted */
  --accent-soft: #e3d4b3;
  --ink-rgb: 26,22,18;
  --paper-rgb: 250,246,238;
  --accent-rgb: 195,162,99;
}
```

**Why this works for RV:** the lightest warm paper in the system. Good for ecommerce-style product grid posts where you want maximum photo brightness. Pair with full-bleed product shots and minimal copy.

---

### Midnight Brass *(the only dark Editorial)*

The **only** dark Editorial palette. Reserved for night photography, candle-lit gifting imagery, jewelry on dark velvet, and any post whose source imagery is already dark and would be diminished by paper backgrounds. Do not improvise other dark palettes — if Midnight Brass does not fit, pick a different mode.

```css
[data-theme="midnight-brass"] {
  --paper:     #14110d;
  --paper-2:   #1f1a13;
  --ink:       #ece2cf;
  --muted:     #9a8c75;
  --line:      rgba(236,226,207,.22);
  --accent:    #d4a04a;     /* gilt brass — gold highlight */
  --accent-soft: #3a2a14;
  --ink-rgb: 236,226,207;
  --paper-rgb: 20,17,13;
  --accent-rgb: 212,160,74;
}
```

**Why this works for RV:** dark backgrounds evoke "unboxing at night," velvet jewelry trays, and moody gift moments. The gilt accent stays warm and metallic — never neon. Use sparingly for hero covers and seasonal drops.

**Midnight Brass must also override two background layers** — light-paper math does not carry over:

```css
[data-theme="midnight-brass"] .grain {
  opacity: .26;
  mix-blend-mode: screen;
  background-image: radial-gradient(rgba(255,244,214,.10) 1px, transparent 1px);
}
[data-theme="midnight-brass"] .paper-wash {
  background:
    radial-gradient(80% 50% at 28% 16%, rgba(212,160,74,.12), transparent 64%),
    radial-gradient(70% 60% at 80% 86%, rgba(60,40,20,.20), transparent 72%),
    linear-gradient(180deg, rgba(236,226,207,.02), rgba(0,0,0,.32));
}
[data-theme="midnight-brass"] .frame-img {
  background: #18120f;
  box-shadow: 0 0 0 1px rgba(236,226,207,.10);
}
```

The seed `template-editorial-card.html` ships these overrides — just switch `data-theme` and they apply automatically.

**Magazine palette rules (Rare Visual specific):**
- Use `--paper` as the main background and `--ink` as primary type.
- Use `--accent` sparingly: section marker, page number, pull quote rule, or one highlighted phrase.
- `--paper-2` can support photo wells, issue strips, or checklist bands.
- Light palettes (the first five): do not turn into beige-on-beige. Maintain real contrast.
- **Never use cream-on-cream**: every warm palette has a deeper `--ink` for that reason. Contrast is non-negotiable.
- Midnight Brass: do not stack opaque cards or fills on the page. Dark Editorial relies on photo bleeds + warm gilt accent for hierarchy, not background blocks.

---

## Swiss International Palettes (4 themes)

Adapted from Guizang's Swiss mode for Rare Visual utility content — material education, FAQ carousels, "how to style" tutorials, gift guides, customer testimonial matrices, and review roundups.

### RV Gold *(default — replaces IKB Blue)*

Default for gift roundups, FAQ posts, "how to wear" tutorials, customer testimonial spotlights, and any structured list-style post.

```css
[data-accent="rv-gold"] {
  --paper:    #faf6ee;
  --ink:      #1a1612;
  --grey-1:   #f0e9da;
  --grey-2:   #d8cfba;
  --grey-3:   #80766a;
  --accent:   #b8924a;     /* RV gold — same as Warm Brass accent */
  --accent-on: #ffffff;
}
```

**Why this works for RV:** the same restrained brass tone as Warm Brass, but in Swiss's strict grid layout. This is the workhorse for utility posts — gift guides, "5 ways to wear," customer review spotlights.

---

### Honey *(replaces Lemon Yellow — warmer, less neon)*

Use for seasonal posts (Valentine's, Mother's Day, holiday), energetic gifting roundups, and any post that wants to feel celebratory without being loud.

```css
[data-accent="honey"] {
  --paper:    #faf6ee;
  --ink:      #1a1612;
  --grey-1:   #f0e9da;
  --grey-2:   #d8cfba;
  --grey-3:   #80766a;
  --accent:   #e8b54d;     /* honey-gold — softer than neon yellow */
  --accent-on: #1a1612;
}
```

**Why this works for RV:** yellow neon fights the brand. Honey-gold sits in the same warm family as RV gold but with more energy. Use for Q4 gift-season content.

---

### Sage *(replaces Lemon Green — natural, not Gen-Z)*

Use for nature/sustainability posts, semi-precious stone spotlights (jade, moss agate, green tourmaline), "spring drops," and any post that wants a calm natural accent.

```css
[data-accent="sage"] {
  --paper:    #faf6ee;
  --ink:      #1a1612;
  --grey-1:   #f0e9da;
  --grey-2:   #d8cfba;
  --grey-3:   #80766a;
  --accent:   #8aa178;     /* sage green — semi-precious moss */
  --accent-on: #ffffff;
}
```

**Why this works for RV:** stones, natural materials, sustainability messaging. Avoid if the post has saturated green product photography (jade saturated against sage will clash).

---

### Brick *(replaces Safety Orange — warm, not industrial)*

Use for Q4 countdown posts, "limited stock" calls, urgent gifting reminders, and any post where you need attention without screaming.

```css
[data-accent="brick"] {
  --paper:    #faf6ee;
  --ink:      #1a1612;
  --grey-1:   #f0e9da;
  --grey-2:   #d8cfba;
  --grey-3:   #80766a;
  --accent:   #b85542;     /* brick-red — terracotta */
  --accent-on: #ffffff;
}
```

**Why this works for RV:** terracotta reads as warm/earthy and ties back to leather and brass — not industrial like Safety Orange. Use sparingly for "last chance" or "limited edition" framing.

---

## Swiss palette rules (Rare Visual specific):

- Use exactly **one** `--accent`.
- **No gradients, no shadows, no glass, no mixed accent colors** — Swiss stays disciplined.
- If the accent is Honey (yellow-gold), text on accent must use `--accent-on: #1a1612` (dark text on light accent).
- Prefer pure blocks, hairline rules, and grid rhythm.
- **Never pair RV Gold accent with chrome/silver text or photography** — they fight. If the photography is silver-toned, switch to Stone Blue editorial instead.

---

## Migration from upstream

| Upstream theme | Rare Visual replacement | Reason |
|---|---|---|
| `ink-classic` (Editorial) | **`warm-brass`** (Editorial) | Default shift from neutral black-on-cream to warm brass-on-cream |
| `indigo-porcelain` (Editorial) | **`stone-blue`** (Editorial) | Same role (analytical), same color family |
| `forest-ink` (Editorial) | **`olive-stone`** (Editorial) | Same role (outdoors/natural), muted to fit RV palette |
| `kraft-paper` (Editorial) | **`warm-brass`** (Editorial) | Merged — RV already has warm brass, no need for a second warm theme |
| `dune` (Editorial) | **`burnished-brass`** (Editorial) | Same role (aesthetic/object study), shifted to brass family |
| `midnight-ink` (Editorial) | **`midnight-brass`** (Editorial) | Same role (dark hero), accent swapped to gilt brass |
| `ikb` (Swiss) | **`rv-gold`** (Swiss) | Default swap from IKB Blue to brand gold |
| `lemon-yellow` (Swiss) | **`honey`** (Swiss) | Same role (energetic), warmer and less neon |
| `lemon-green` (Swiss) | **`sage`** (Swiss) | Same role (eco/natural), muted to fit RV palette |
| `safety-orange` (Swiss) | **`brick`** (Swiss) | Same role (attention), terracotta instead of industrial orange |

If you have existing local tests using upstream theme names, run the rename before re-rendering:

```bash
# Quick sed-based rename for legacy local tests
sed -i 's/ink-classic/warm-brass/g; s/indigo-porcelain/stone-blue/g; s/forest-ink/olive-stone/g;
        s/kraft-paper/warm-brass/g; s/dune/burnished-brass/g; s/midnight-ink/midnight-brass/g;
        s/data-accent="ikb"/data-accent="rv-gold"/g;
        s/lemon-yellow/honey/g; s/lemon-green/sage/g; s/safety-orange/brick/g' \
    local-tests/*/index.html
```

---

## When in doubt

- Default to **`warm-brass`** Editorial for product photography and lifestyle covers.
- Default to **`rv-gold`** Swiss for utility posts and gift guides.
- Reach for **`midnight-brass`** only when the imagery is already dark and warm.
- Reach for **`stone-blue`** only when the post needs credibility and clarity over warmth.

> Reminder: Rare Visual's brand voice prefers warm, grounded, effortless. Reach for cold or neon palettes only when the content explicitly calls for them.