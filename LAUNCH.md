# DevToolbox — Launch & Growth Checklist

Live: https://weather-source.github.io/dev-toolbox/

## Market evidence (researched 2026-10-25)
- jsonformatter.org (single-purpose tool site, ad-monetized): **~3.87M visits/month** (Semrush), 42% from Google organic → the "online dev tool" niche is proven and monetizable.
- Competitors monetize via AdSense + affiliate; most upload data to servers — our differentiator is **100% client-side privacy**.

## Week 1 — Free launch channels (0 cost)
- [ ] **Google Search Console**: add property `weather-source.github.io/dev-toolbox/`, submit `sitemap.xml`, request indexing for all 18 tool pages.
- [ ] **Bing Webmaster Tools**: same (imports from GSC).
- [ ] **tiny-helpers.dev**: submit via GitHub PR to `stefanjudis/tiny-helpers` repo (add JSON entry for our tools).
- [ ] **AlternativeTo**: open submit form (no account needed) — list DevToolbox as alternative to jsonformatter.org, crontab.guru, regex101.
- [ ] **Show HN** (news.ycombinator.com): "Show HN: DevToolbox – 18 privacy-first dev tools, no server, no signup".
- [ ] **Reddit**: r/webdev, r/InternetIsBeautiful, r/tools (follow each sub's self-promo rules; lead with the privacy angle).
- [ ] **V2EX / 掘金 / NodeSeek** 中文社区：以"纯前端、无上传"卖点发介绍帖.
- [ ] Launch directories: get100users.app lists 31 free ones (Uneed, Starter Story alternatives, etc.).

## Monetization (in order)
1. **Buy Me a Coffee** — button already on every page; register at buymeacoffee.com, then replace the placeholder URL (grep `buymeacoffee.com/` across HTML, one commit).
2. **Google AdSense** — every page has `.ad-slot` placeholders; privacy.html is ready for review. Apply after 2–4 weeks of content/traffic. Replace ad-slot divs with AdSense `<ins>` tags.
3. Optional later: GitHub Sponsors link in footer.

## SEO already in place
- Per-page canonical + Open Graph + Twitter card
- JSON-LD: WebSite (index) + FAQPage (index FAQ)
- sitemap.xml (22 URLs, absolute), robots.txt, custom 404
- FAQ section with 5 questions (wins rich snippets)

## Maintenance
- All code is static HTML/CSS/vanilla JS in this repo. `git push` auto-deploys via GitHub Pages (build takes ~1 min).
- No server, no cost, no dependencies except qrcode-generator on jsDelivr.

## Tool ideas for round 2 (by search demand)
- Word/character counter, JWT *builder*, JSON↔YAML, HTML/CSS/JS minifier, URL parser/query editor, slug generator, random data (faker-lite) generator, cron-to-human translator variations, PNG→JPG/WebP batch, base64 image data-URI converter.
