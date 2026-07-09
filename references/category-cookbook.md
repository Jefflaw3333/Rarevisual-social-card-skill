# Category Cookbook

> Fork of `guizang-social-card-skill` v0.15, rebranded for **Rare Visual** (rarevisual.com) — a premium handcrafted accessories DTC brand for women 25–45 in the US. Voice: *"Handcrafted accessories that turn everyday outfits into something intentional."*

Per-category cheat sheet for the **11 content categories** this skill routes for Rare Visual. Each entry maps a category to:

- **What we can do** — concrete poster types this skill produces well for RV.
- **Capability** — which side of the 3-bucket circle this category lands in.
- **Recipes** — which layout IDs (M01–M16 / S01–S12) are first reach.
- **Style mode** — which side of the system (Editorial / Swiss) and which theme preset fits.
- **Text scheme** — how text relates to image (text-on-image / text-beside-image / text-only).
- **Image source** — where the photos come from (RV catalog, user-supplied, web).
- **Content shape** — page count and page-by-page structure.
- **Pitfalls** — the way this category breaks for an accessories brand.

This is a routing document. When the user names a category, find the row here and start from the listed recipes instead of building from a blank file.

For any category, if a poster has a full-bleed image with text on top, also follow `image-overlay.md` (photo qualification, localized tint fallback, and subject avoidance).

---

## Rare Visual Category Capability

This is the **RV-flavored** version of the capability circle. Use it to triage any incoming brief before picking recipes.

### Bucket 1 — Strong end-to-end (text + structure + image story all in scope)

The skill can produce these posts from a brief alone, including a coherent image story:

| Category | Why it's strong |
| --- | --- |
| 穿搭 · Styling / Outfit Pairings | We can render the jewelry + outfit pairings in Editorial warm-brass or Swiss IKB. The "5 ways to wear one piece" or "work-to-dinner" format maps cleanly to S11 ledger + M02 detail crops. |
| 推荐 · Gift Guides | "Best for her / mom / bridesmaid / anniversary" is a structured product recommendation problem → S12 matrix + S11 ledger + M04 pull-quote pull the whole thing off. |
| 职场 · Work Styling | Office-to-evening accessorizing is data-shaped: "5 accessories for the office", "what to wear under a blazer" → S11 ledger + M16 image-led cover. No body shots required. |

### Bucket 2 — Strong copy + structure; image story needs user or curated RV catalog

These posts work well, but you must source the imagery carefully — RV catalog flat-lays or user-supplied travel/vanity photos:

| Category | Why it's partial | What unblocks it |
| --- | --- | --- |
| 旅行 · Styled Travel / Destination | Text/structure fine; the destination photo is the whole story. | User trip photo, or RV catalog flat-lay styled on a hotel tray or beach towel. |
| 家居 · Vanity / Jewelry Storage | "How I store my jewelry" or "vanity setup" is on-brand. | User vanity photo, or staged flat-lay of jewelry on a tray/dish. |

### Bucket 3 — Outside scope (push back honestly)

Be explicit with the user. Do not promise a result the system was not designed to make:

- **游戏 · Game** — not an accessories topic. No RV use case.
- **影视 · Film & TV** — not an accessories topic. Only accept if the user can frame it around a styling moment (e.g. "get the look from the show"). Otherwise push back.
- **彩妆 · Makeup** — different category. Only accept the small overlap (e.g. "earring + lipstick color pairing" or "statement jewelry with minimal makeup") — never as a general makeup tutorial.
- **健身 · Fitness** — never combine jewelry + gym (chain damage, snagging, sweat tarnishing). Push back if asked.
- **情感 · Emotion / 氛围感** — pure atmospheric mood posts (dreamcore, hazy lights, glowy ovals) are explicitly banned by the anti-pattern list. Only accept **anchored** emotional angles: "anniversary gift essay", "treat-yourself self-purchase story", "what jewelry I wore at my wedding".
- **穿搭 · OOTD full-body shots** — daily OOTD needs real body photography. The skill does not generate body shots. Refer to a photography workflow, not this skill.

---

## RV Content Pillars

Every RV social card should ladder up to one of these 5 brand pillars. Pillars are how the brand repeats across channels; categories are how the user finds the post. Map pillar → card mode so we never publish a card that doesn't connect to brand strategy.

| Pillar | What it's about | Best card modes | First-reach recipes |
| --- | --- | --- | --- |
| **Handcraft & Materials** | Education on gold-filled vs gold-plated vs solid brass; care guides; why small-batch matters. | Material breakdown, comparison ledger, myth-busting. | S02 (two-signal comparison) · S11 (specs ledger) · M14 (process pipeline) · M04 (manifesto pull-quote) |
| **Styling & Outfit Pairings** | "5 ways to wear one necklace", work-to-dinner, capsule wardrobe accessories, season pairings. | Styling lookbook, capsule ledger, work-to-evening transitions. | M16 (image-led cover) · S11 (item ledger) · S12 (matrix) · M02 (field-note detail) |
| **Gifting Excellence** | Gift guides by recipient (her, mom, bridesmaid, wife, friend), by occasion (anniversary, birthday, wedding, graduation), by price tier. | Gift matrix, "best of" roundups, occasion-specific hero pages. | S12 (recipient × price matrix) · S11 (price-anchored ledger) · M16 (hero cover) · M07 (closing note) |
| **Behind the Scenes** | Artisan process, small-batch production, founder essay, sourcing story, packaging unboxing. | Process essay, BTS photo story, founder pull-quote. | M11 (marginalia essay) · M14 (process pipeline) · M02 (BTS photo) · M09 (thesis) |
| **Customer Stories** | Real testimonials, real reviews, real wearer essays, UGC reshares. | Review quote card, testimonial ledger, customer photo story. | M04 (pull-quote review) · M13 (hero question) · S11 (review ledger) · M07 (closing note) |

> **Rule of thumb:** if a brief doesn't naturally ladder to one of these 5 pillars, it's probably outside RV's brand territory — push back rather than force-fit.

---

## Live Photo Scene Library

This is not a fixed template list. When the user supplies video, infer the scenario and information budget from the actual content, then choose single Live Photo, triple collage, long-video trimming, or a non-Live-Photo fallback.

Use `references/live-photo-production.md` for duration limits and rendering details. This section only decides what kind of motion is worth showing.

| Scenario | User problem | Motion value | Best Live Photo form |
| --- | --- | --- | --- |
| Jewelry close-up / 手作展示 / unboxing | A still photo cannot prove texture, weight, or scale | show the catch of light on metal, the way it moves, the clasp clicking shut | single `5s`; triple collage for the same piece from 3 angles |
| Outfit pairing / 穿搭 | One styled photo is one opinion, not the full story | show the piece on the body, on the hand, then close-up of the metalwork | triple collage for one piece in 3 contexts; single for one signature look |
| Travel styling / 旅行 | A pretty destination photo has atmosphere but no jewelry story | show piece being worn at destination, then a flat-lay on a hotel tray or beach surface | single `5s`; triple collage for "packing → arrival → worn at dinner" |
| Lifestyle / vanity setup / 家居 | Object photos feel too staged | show the jewelry tray in use, drawer opening, the clasp clicking shut | single `5s`; triple collage for "morning vanity → day worn → evening stored" |
| Gift unboxing / 推荐 | Product photos don't prove the gifting moment | show unwrapping, the card reveal, the first-try-on reaction | single `5s`; triple collage for "boxed → unwrapped → worn" |
| Work-to-evening / 职场 | One styled office look doesn't show the transition | show office look → remove a layer / add a piece → dinner look | triple collage for the 3 stages of the transition |
| Process / 手作过程 (BTS) | Finished photo misses the satisfying craft detail | show pour, file, polish, set, or final reveal | single `3-5s`; avoid showing the full making process in one Live Photo |

Motion role shortcuts:

- **One action point** → single Live Photo, usually `3s` WeChat or `5s` Xiaohongshu.
- **One small process** → single `5s`, possibly with light speed-up.
- **Three parallel results / viewpoints / stages** → triple Live Photo collage.
- **Long sequence or narration-heavy content** → diagnose first; trim, split, or recommend normal video/GIF.

---

## 旅行 · Styled Travel / Destination

**Bucket 2** — strong copy + structure; needs user or curated RV imagery.

- **Recipes**: M01 (text-led cover, no photo dominance) **or M16 (image-led cover, when the user has a destination flat-lay of jewelry)** → M02 (field-note close-up of a piece worn in destination) → M11 (marginalia essay) → M07 (closing note) → S11 (packing-list ledger). For image-heavy submissions use the M16 → S11/M05 → M02 sequence in `references/content-planning.md`.
- **Style mode**: Editorial × warm-brass (default) for warm-tone destinations (Tulum, Lisbon, Marrakech). Editorial × burnished-brass for sun-bleached coastal. Editorial × olive-stone for mountain / wilderness. Swiss × rv-gold only for "packing checklist data" style posts.
- **Text scheme**: Text beside image is the default. Cover can use text-on-image only when the photo has a quiet zone; add localized tint only if the thumbnail check fails. Body pages use photo + caption pairs (field-note style).
- **Image source**: User destination photos (with their jewelry in frame) > RV catalog flat-lays on hotel trays / stone surfaces > Unsplash (`/s/photos/<destination>`, best for overseas / English keywords) > Flickr CC (`license=2,3,4,5,6,9`, when you need documentary "real trip" feel rather than postcard polish). Always log to `assets/SOURCES.md`.
- **Content shape**: 5–7 pages. Cover (destination + jewelry in shot) → atmosphere photo + lead → packing-list ledger (which pieces to bring) → 2–3 field notes (one location each, piece styled in destination) → closing quote / next-stop teaser.
- **Pitfalls**:
  1. **Destination without jewelry** — a postcard-style travel cover with no piece in frame. Cure: every page must show the jewelry being worn or staged in destination, not just the place itself.
  2. **Generic "best places in X city" listicle voice.** Cure: keep one specific date / weather / outfit detail per page to anchor it as observed, not researched.
  3. **Cross-promoting a trip the user didn't take.** Stock-photo-only travel posts feel aspirational in the wrong way for a DTC brand — the promise is "this is what an RV piece looks like in real life".

---

## 职场 · Work Styling

**Bucket 1** — strong end-to-end. This is one of RV's three core formats.

- **Recipes**: S01 (cover) · S02 (work vs dinner comparison) · S11 (5-accessories-for-the-office ledger) · M16 (image-led cover for "the one piece that changes everything") · S07 (takeaway ledger) · M11 (work-to-evening essay marginalia).
- **Style mode**: Editorial × warm-brass for the default office look. Swiss × rv-gold for "office data" / capsule accessory counts. Avoid honey / sage for serious work-styling content; they read as marketing.
- **Text scheme**: Text-beside-image is default (small jewelry crop + outfit note). Almost never text-on-photo for body pages. Cover can use text-on-image if the cover photo has a quiet zone.
- **Image source**: RV catalog flat-lays of pieces on neutral office surfaces (folded blazer, linen tote, ceramic mug) > user office photos. Avoid stock business photos — handshake, laptop-with-coffee. If you need an image, prefer a flat-lay or omit.
- **Content shape**: 5–9 pages. Cover (one piece + claim like "the only accessory you need at 9am and 7pm") → "5 accessories for the office" ledger → work-to-dinner transition diagram (S02 or M02) → styling tips marginalia → closing takeaway.
- **Pitfalls**:
  1. **Listicle voice** ("8 accessories for the office"). Cure: each row makes a falsifiable claim ("Layered under a blazer, the Audrey chain disappears — pull the collar, and it's the whole outfit"), not generic advice.
  2. **Cheap "advice" energy** — soft language ("一定要", "千万别"). Cure: replace with observed action verbs and a specific piece name.
  3. **Stock-photo seasoning** — handshake, laptop-with-coffee, woman-at-desk. Cure: omit, or use a small Lucide icon glyph instead.
  4. **Pure office-only framing.** RV's "work-to-dinner" angle is the strongest — never close a work post without an evening transition.

---

## 游戏 · Game

**Bucket 3 — Outside scope.** Not an RV content category.

- **Recipes**: none first-reach.
- **Style mode**: n/a.
- **Text scheme**: n/a.
- **Image source**: n/a.
- **Content shape**: n/a.
- **Push-back line**: "Game content isn't on Rare Visual's content map. If you want to talk about a styling moment from a game/show (e.g. jewelry in a game character design), reframe the brief as 穿搭 or 推荐 and we can produce it. Otherwise we should not publish this."

---

## 影视 · Film & TV

**Bucket 3 — Outside scope**, with a narrow accept-criteria exception.

- **Acceptable only when**: the user can anchor the post to a styling moment — "get the look from [show/film]", "the jewelry in [period drama]", "what I'd wear to a [show] premiere". Reframe as 穿搭 or 推荐 in those cases.
- **Recipes** (when accepted): M04 (pull quote for a memorable styling line) · M10 (evidence feature for jewelry-on-character analysis) · M11 (marginalia essay) · S02 (two-signal comparison of two styling moments) · S12 (matrix for "best jewelry moments in [show]").
- **Style mode**: Editorial × warm-brass or × stone-blue for the styling-essay angle.
- **Text scheme**: Text-beside-image for review cards (still + take). Text-on-image only for atmospheric "what this styling made me feel" quote pages.
- **Image source**: Official stills / press photos only. Do not generate fake stills.
- **Content shape**: For single show styling: cover (title + styling take) → 1–2 scene captures → director / costume-design pull-quote → verdict ledger of pieces.
- **Pitfalls**:
  1. **Generic review voice** ("this film is a masterpiece"). Cure: anchor every claim to one styling detail and one RV-relevant takeaway.
  2. **Spoiler in title without warning.** If a cover gives away the ending or a styling reveal, mark `剧透` in the kicker.

---

## 美食 · Food

**Bucket 3 / 边缘 Bucket 2** — only the narrow RV crossover is acceptable (table styling, gold cutlery, hosting).

- **Acceptable**: gold cutlery flat-lay, tablescape styling with jewelry as the centerpiece, "hosting jewelry" (statement earrings for dinner parties, bracelets that don't catch on linen, necklaces that sit above a high neckline). Treat as a 家居 / 穿搭 crossover, not as a food post.
- **Not acceptable**: recipes, restaurant reviews, drool-shot art direction, finished-dish hero photos. RV does not do food.
- **Recipes** (when accepted): M16 (image-led cover with gold cutlery flat-lay) → S11 (tablescape ledger) → M02 (detail crop of a piece worn at the table) → M07 (closing hosting tip).
- **Style mode**: Editorial × warm-brass or × ivory. The cookware-on-linen vibe fits.
- **Text scheme**: Text-with-image. The tablescape is one frame; everything else is text/data.
- **Image source**: RV catalog flat-lay (gold cutlery + brass jewelry on linen) > user hosting photos. Stock food photos read as Western stock and break the brand trust signal.
- **Push-back line** for non-crossover food posts: "Food content isn't on Rare Visual's content map. If you have a hosting / tablescaping angle with jewelry in frame, we can produce that as a 家居 or 穿搭 crossover."

---

## 彩妆 · Makeup

**Bucket 3 — Outside scope**, with a narrow makeup-jewelry crossover exception.

- **Acceptable only when**: the user frames the post as a makeup + jewelry pairing — "the earrings that disappear under a red lip", "no-makeup makeup with statement jewelry", "what to wear when your makeup is the look". The jewelry is the hero; the makeup is the supporting frame.
- **Not acceptable**: full makeup tutorials, "get the look" posts requiring a recognizable model face, color-swatch breakdowns, foundation shade matching. RV is not a beauty brand.
- **Recipes** (when accepted): S11 (jewelry-led ledger with a small makeup note column) · M02 (pairing detail crop) · M04 (manifesto pull-quote on "less makeup, more metal"). Do not use M14 as a makeup tutorial pipeline.
- **Style mode**: Editorial × warm-brass or × stone-blue for the jewelry-hero pairing.
- **Text scheme**: Text-beside-image — small jewelry hero, small makeup crop, one sentence on the relationship.
- **Image source**: User pairing photos. Stock makeup photos have legal grey areas and look generic.
- **Pitfalls**:
  1. **Color-swatch inaccuracy** if you eyeball CSS hex from a photo. Always ask the user for the official shade name + hex.
  2. **Sliding from jewelry × makeup pairing into a generic makeup tutorial.** If the brief becomes "5-step night-out makeup", push back.

---

## 健身 · Fitness

**Bucket 3 — Outside scope.** Never combine jewelry + gym.

- **Push-back line**: "We don't pair Rare Visual jewelry with fitness content — chains snag, metal tarnishes with sweat, and the brand promise is 'intentional everyday wear', not workout gear. If you want to talk about post-workout styling or recovery-day jewelry (e.g. what's safe to leave on for a walk, a yoga class that's low-impact), we can frame that as 穿搭 — but no gym hero shots, no progress photos, no before/after."
- **Recipes**: none. Do not use S09, M14, M15 for RV.

---

## 家居 · Vanity / Jewelry Storage

**Bucket 2** — strong copy + structure; image story needs user or RV catalog.

- **Recipes**: M16 (image-led cover when user has a strong vanity photo) → S11 (storage ledger with price) → M02 (detail crops of trays, dishes, drawer inserts) → M11 (marginalia on "my morning jewelry routine"). Also M15 (before/after — needs paired user photos for a vanity transformation), M03 (essay-style "how I store my jewelry" manifesto).
- **Style mode**: Editorial × warm-brass or × ivory for warm linen/wood vanity setups. Editorial × stone-blue for cool modern marble. Swiss × rv-gold for "vanity data" posts (counting pieces by category, cost per storage slot, etc.).
- **Text scheme**: Item recommendations are text-beside-image (small product crop + name + price + reason). Before/after is two photos with mid-page divider. Storage ledger rows are text + small thumbnail.
- **Image source**: User vanity photos (best — the storage context is personal) > RV catalog flat-lays of jewelry on trays/dishes/stands > carefully attributed Unsplash for vanity scene backgrounds.
- **Content shape**: Vanity rec — cover (vanity style + budget) → 4–6 storage item rows ledger → 1 hero detail crop → closing tip. Storage routine — cover → "morning routine" ledger → 1–2 detail crops → closing note.
- **Pitfalls**:
  1. **Pinterest-aesthetic stock** that the user can't actually reproduce (marble vanities, walk-in closets). Stick to what real RV customers live in: a tray on a dresser, a dish on a nightstand, a small ring holder.
  2. **Price drift** — products move quickly. Don't quote a price more than 90 days old without re-checking.
  3. **Straying into interior design** (full room makeovers, paint colors, furniture). Reframe those posts to "vanity corner" scope.

---

## 穿搭 · Styling / Outfit Pairings

**Bucket 1 — strong end-to-end.** This is RV's core category. Map every styling post to the **Styling & Outfit Pairings** pillar.

- **Recipes**: M16 (image-led cover) → S11 (capsule accessory ledger — "5 pieces, 7 outfits") → S12 (item matrix: piece × occasion) → M02 (outfit detail crop) → M11 (marginalia essay — "this week I wore") → M04 (style manifesto pull-quote) → M07 (closing note). For "5 ways to wear one piece", use S11 ledger with 5 styled rows + 1 hero detail.
- **Style mode**: Editorial × warm-brass (default) for everyday styling. Editorial × warm-brass or × stone-blue for editorial-feel essays. Editorial × burnished-brass for sun-bleached summer styling. Swiss × honey / Safety Orange for capsule-wardrobe data posts ("the 7-piece accessory capsule that covers a workweek").
- **Text scheme**: Text-beside-image — small jewelry + outfit crops as evidence, one full-body hero only if user provides. Cover can use text-on-image with quiet-zone tint if the photo supports it.
- **Image source**: User OOTD photos (we don't generate body shots — be honest about this). For mood-board context, RV catalog flat-lays (piece on linen, on stone, in styled tray) work well and stay on-brand. Web-sourced flat-lays okay with disclosure.
- **Content shape**:
  - **Capsule guide** — cover (season + piece count) → wardrobe ledger → 1–2 outfit demonstrations → care/styling marginalia.
  - **"5 ways to wear"** — cover (one hero piece) → 5 styled rows with different necklines / layers / occasions → closing styling tip.
  - **Work-to-dinner** — cover (one piece, one claim) → 9am look → 7pm look → S02 comparison → closing tip.
- **Pitfalls**:
  1. **Brand-and-price-tag overload** turning every poster into an ad. Limit to 6 named pieces max, and only on the ledger pages.
  2. **Daily OOTD posts.** The skill cannot generate body photography. Push the user to a photography workflow, or accept RV catalog flat-lays only.
  3. **Generic "minimalist 25 件夏季基础款" listicle.** Cure: anchor to a specific climate / lifestyle constraint ("the 6-piece accessory capsule for hot, humid Singapore offices").
  4. **High-styling editorial fashion shoots.** Requires real photography production. The skill produces the styling *narrative*, not the shoot.

---

## 情感 · Emotion / Personal Essay

**Bucket 3 — Outside scope for atmospheric mood**, with a narrow accept-criteria exception for anchored emotional angles.

- **Acceptable only when** the brief has a concrete RV anchor:
  - Anniversary gift essay ("what I bought my mom for her 60th")
  - Self-purchase "treat yourself" story
  - Wedding / bridesmaid jewelry essay
  - Memorial or heirloom piece story
  - Founder / artisan personal essay

  Map these to the **Behind the Scenes** or **Customer Stories** pillar, not to the 情感 category as a whole.

- **Not acceptable**:
  - "梦核 / 氛围感" with soft fluorescent gradients, glowing ovals, hazy lights. The anti-pattern list explicitly bans those decorations.
  - Y2K / 早期网络回忆 / 千禧辣妹 aesthetic.
  - Heavy emoji / kaomoji captions. We use no emoji.
  - Inspirational generic copy ("愿你...愿我..."). Editorial demands specifics — name the day, the weather, the piece.
- **Recipes** (when accepted): M04 (pull-quote / thesis) · M09 (atmospheric thesis) · M11 (marginalia essay) · M13 (hero question — for rhetorical-question covers) · M07 (closing note) · M02 (one quiet supporting photo — a hand, a window, a piece on a dresser).
- **Style mode**: Editorial × warm-brass (default) or × warm-brass. Magazine pace with restraint.
- **Text scheme**: Mostly text-only with one quiet supporting image. The text is the content; the image is evidence.
- **Image source**: Quiet documentary-style photo — user-supplied is best. RV catalog flat-lays of a single piece on linen work as the quiet supporting image. If sourcing: **Flickr CC** (`license=2,3,4,5,6,9`) is the strongest match for real interiors, real hands, real moments without stock polish. Avoid the "moodcore" gradient-light stock entirely.
- **Content shape**: 3–5 pages. Cover question → essay split (M03) or atmospheric thesis → pull quote → closing note. Resist over-stretching to 9 pages.
- **Pitfalls**:
  1. **Inspirational generic copy.** Cure: name the day, the weather, the person, the piece.
  2. **Pretty empty space** — page after page of one pullquote on paper. Risk: reads as filler. Mix with one M02 field photo or M11 marginalia to ground it.

---

## 推荐 · Gift Guides / Recommendations

**Bucket 1 — strong end-to-end.** This is RV's second core category. Map every 推荐 post to the **Gifting Excellence** pillar.

- **Recipes**: M16 (image-led hero cover with a single hero piece or "best of" cover) → S12 (recipient × price matrix, e.g. mom × under $50 / under $100 / under $200) → S11 (gift ledger with 4–8 pieces, price-anchored) → M02 (one detail crop per hero piece) → M04 (closing pull-quote: "the one piece I'd gift if I could only gift one"). Also S02 (two-signal comparison: "for mom vs for friend", "for bridesmaid vs for wife") and S07 (takeaway ledger).
- **Style mode**: Editorial × warm-brass (default) for "best for her / mom". Editorial × burnished-brass for collection roundups and "best of" lists with more drama. Swiss × rv-gold for the data-shaped version ("12 gifts under $100, ranked by re-purchase rate"). Swiss × brick only for price-comparison urgency posts.
- **Text scheme**: Hero cover text-on-image with quiet-zone tint. Body pages text-beside-image (small piece crop + name + price + 1-line "why this piece"). The piece is the visual evidence; the text is the recommendation reasoning.
- **Image source**: RV catalog flat-lays are the workhorse. One piece, one styled surface (linen, marble, leather). User photos only when the brief is "I gifted this and here's the reaction".
- **Content shape**:
  - **By recipient** — "Best gifts for mom / bridesmaid / wife / friend / the woman who has everything": cover → recipient matrix → 4–6 piece rows → closing tip.
  - **By occasion** — "Anniversary / birthday / graduation / wedding / bridal shower": cover → occasion matrix → 4–6 piece rows → closing tip.
  - **By price tier** — "Best under $50 / $100 / $200": cover → price tier matrix → 4–6 piece rows → closing tip.
  - **The one piece** — hero recommendation: cover → one piece hero → 3 reasons → closing pull-quote.
- **Pitfalls**:
  1. **Generic "top 10 gifts" listicle.** Cure: anchor to a specific recipient or occasion with one observable detail ("for the mom who keeps her jewelry in a ceramic dish by the bed").
  2. **Price drift** — gift posts get shared for months. Re-check all prices before publishing.
  3. **Out-of-stock pieces.** Don't include a piece you can't link to a buyable URL. Filter the ledger to in-stock pieces only.
  4. **All pieces, no recommendation.** A list of 12 SKUs is not a gift guide. The guide must make a case for each piece.

---

## Rare Visual Category Capability — Summary

A compact reference of the 3-bucket circle, RV-flavored:

**Strong end-to-end (text + structure + image story all in scope):**

- 穿搭 · Styling / Outfit Pairings
- 推荐 · Gift Guides
- 职场 · Work Styling

**Strong copy + structure; image story needs user or curated RV catalog:**

- 旅行 · Styled Travel / Destination
- 家居 · Vanity / Jewelry Storage

**Outside scope (push back honestly):**

- 游戏 · Game
- 影视 · Film & TV (accept only as 穿搭 / 推荐 crossover)
- 彩妆 · Makeup (accept only as jewelry-makeup pairing)
- 健身 · Fitness
- 情感 · Atmospheric 氛围感 / dreamcore (accept only anchored emotional angles)
- 穿搭 · Daily OOTD full-body shots
- 美食 · Food (accept only tablescape / gold cutlery crossover)
- Any post requiring high-saturation Y2K / 千禧辣妹 / dolly / kawaii decoration vocabulary
- Pure photography showcase posts where the image is the entire product

**Be explicit with the user when their request lands in the "outside scope" bucket. Do not promise a result the system was not designed to make.** When in doubt, reframe the brief to the nearest in-scope category rather than forcing it into the wrong one — RV's brand consistency depends on every card laddering to one of the 5 content pillars.
