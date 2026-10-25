# DevToolbox

Free, private, browser-based developer tools. Static site — no backend, no tracking, nothing leaves the user's browser.

**Live:** https://weather-source.github.io/dev-toolbox/

## Tools

| Tool | Page | Highlights |
|---|---|---|
| Cron expression generator | `/cron.html` | Full 5-field parser (ranges, steps, lists, names), plain-English explanation, next 5 run times |
| Regex tester | `/regex.html` | Live match highlighting, capture groups, replace preview |
| JWT decoder | `/jwt.html` | Header/payload decode, expiry check, exp/iat/iss/sum claims |
| Timestamp converter | `/timestamp.html` | s/ms auto-detect, both directions, relative time |
| Password generator | `/password.html` | Web Crypto API, entropy estimate, ambiguous-char stripping, passphrase mode |
| Image compressor | `/image-compressor.html` | Canvas-based compress + resize, JPEG/WebP/PNG, drag & drop |
| Color converter | `/color.html` | HEX/RGB/HSL, tints & shades palette, WCAG contrast |
| QR code generator | `/qrcode.html` | Text/URL/Wi-Fi/mailto, 4 ECC levels, PNG download |

## Tech

Plain HTML/CSS/vanilla JS. One CDN dependency (qrcode-generator via jsDelivr). Hosted on GitHub Pages.

## Monetization

- Ad slots (`<div class="ad-slot">`) reserved on every page — drop in AdSense `<ins>` tags after approval.
- Buy Me a Coffee donation buttons on every page.

## Local dev

Open any page directly in a browser, or `python -m http.server` from this directory.
