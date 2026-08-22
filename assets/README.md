# Bar Mario — Asset Handoff Guide

The original file embedded large base64 assets, which have been removed. This site uses a lightweight CSS aperitivo-ledger treatment until approved business imagery is available. It contains no generated food imagery, stock food imagery, remote placeholder images, or encoded asset data.

| Suggested file | Use | Recommended treatment |
|---|---|---|
| `logo/bar-mario-logo.svg` | Crisp header brand mark / favicon source | Approved SVG or transparent PNG. Do not paste a screenshot or base64 string. |
| `hero/bar-mario-room.webp` | Optional hero atmosphere/storefront image | Approved real photo, landscape WebP, about 1600px wide and compressed. |
| `gallery/bar-mario-bar.webp` | Optional below-fold bar photo | Approved real photo, responsive WebP, lazy-load below the fold. |
| `gallery/bar-mario-dining-room.webp` | Optional below-fold dining-room photo | Approved real photo, responsive WebP, lazy-load below the fold. |
| `social/bar-mario-social-preview.jpg` | Social sharing card | Approved 1200 × 630px JPG/PNG. |

Update the adjacent `<!-- ASSET: ... -->` comments in `index.html` when approved assets are supplied. Never use base64 embedding, unapproved restaurant photography, generic stock food, or AI-generated food imagery as a replacement.

## Premium visual treatment

| File | Purpose | Public-facing constraint |
|---|---|---|
| `visuals/aperitivo-light-study.svg` | Local abstract aperitivo-light material used behind the homepage’s refractive 3D stage | Do not represent it as the restaurant, food, menu, staff, guests, inventory, service outcomes, or a real Bar Mario mark. It is a non-documentary decorative treatment only. |

Keep the hero contrast overlay and the motion-independent reservation and ordering actions in `index.html` when replacing this visual treatment. The CSS refractive facets are an abstract material effect, not a menu or restaurant photograph.
