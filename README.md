# Bar Mario

A single-page website for **Bar Mario**, an Italian bar and kitchen at 365 Van Brunt St in Red Hook, Brooklyn. One static `index.html`, no framework, no build step, deployed to GitHub Pages.

**Live site:** https://oumark24.github.io/Bar-Mario-Test-Run/

## What it does

- **Scroll-reveal sections** built on `IntersectionObserver` with a graceful fallback: if the browser lacks the API *or* the visitor has `prefers-reduced-motion: reduce` set, every section is simply revealed immediately instead of animating. No content is ever hidden behind an animation that might not run.
- **Menu, room and drinks sections** for a Piedmontese/Tuscan menu, written to match how the bar actually describes itself rather than generic restaurant filler.
- **DoorDash hand-off** for delivery orders.
- **Full SEO surface** — `Restaurant` JSON-LD with address and phone, Open Graph and Twitter card tags, plus a committed `robots.txt` and `sitemap.xml` pointing at the canonical Pages URL.
- **Responsive layout** across 12 media-query breakpoints, and 5 `aria-label`s on the interactive controls.

## Why it's built this way

A bar's website has one job: convince someone to come in, then tell them where it is. That fits in one file. Keeping it framework-free means no build step to break and no dependency to update, and GitHub Pages hosts it for free.

The `IntersectionObserver` fallback is the part worth pointing at — animation is treated as an enhancement, so the page is fully readable even when the animation path never runs.

## Running it

```bash
git clone https://github.com/Oumark24/Bar-Mario-Test-Run.git
cd Bar-Mario-Test-Run
open index.html
```

## Deployment

`.github/workflows/static.yml` publishes the repository root to GitHub Pages on every push to `main`.

## Files

| Path | Purpose |
| --- | --- |
| `index.html` | Entire site — markup, CSS, scroll-reveal logic |
| `robots.txt` | Crawler rules and sitemap pointer |
| `sitemap.xml` | Canonical URL for search engines |
| `.github/workflows/static.yml` | GitHub Pages deployment |
