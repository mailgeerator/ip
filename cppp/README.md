# PrivyTools

All-in-One Privacy & Utility Toolkit: Temporary email, latest user-agent generator, IP checker with sample ZIP/phone, URL shortener, and email validator. Built with vanilla TS/JS, HTML, and CSS for speed and clarity.

## Features
- Temporary email generator with client-side inbox (simulated provider)
- Latest User-Agent generator (desktop, iOS, Android; Chrome/Safari/Firefox and in-app browsers)
- IP checker with geodata, plus random ZIP/phone examples by country
- URL shortener with base62 codes and redirects
- Email validator with syntax, typos, and disposable detection
- Google AdSense slots (header, sidebar, footer)
- SEO best practices, sitemap and robots

## Tech
- Frontend: HTML, CSS, TypeScript (compiled to JS)
- Optional serverless API: Node (Vercel/Netlify/Fly/Cloudflare)
- Storage: localStorage/IndexedDB; optional KV/SQLite for shortener

## Development
1. Open `index.html` (from `src/pages/`) via local server (recommended).
2. Any static server works, e.g., `npx serve src` or VSCode Live Server.
3. Update AdSense `data-ad-client` and `data-ad-slot` in `src/scripts/adsense.js` or per-page ad slots.

## Build
No heavy build required. If you want TypeScript, compile with `tsc` or embed via `<script type="module">` using plain JS.

## Deploy
- Upload `src` and `public` to any static host (Netlify, Vercel static, GitHub Pages). If using serverless, deploy `/api` to your platform.

## Security
- Strict Content-Security-Policy via meta tags
- No inline scripts/styles; all JS/CSS external
- Input sanitization for URLs, emails, and HTML rendering

## License
MIT
