# EcoSwap Adelaide — DMIP Part B

A five-page, mobile-responsive **student demonstration** of a sustainable local reuse marketplace, built with HTML, CSS and vanilla JavaScript.

## Pages
- `index.html` — Home
- `about.html` — About
- `browse.html` — Browse demo listings (search, category filters, price sorting)
- `how-it-works.html` — How It Works
- `contact.html` — Contact (front-end demo form; does not send or store messages)

## Local preview
Open `index.html` in a browser. For a local server, run `python -m http.server 8000` from the project folder and open `http://localhost:8000`.

## Publish to GitHub Pages
1. Sign in to GitHub and create a **public** repository, e.g. `ecoswap-adelaide`.
2. Upload **all five HTML files**, `assets/`, and `README.md` to the repository root (not a nested folder).
3. Open **Settings → Pages → Build and deployment**. Choose **Deploy from a branch**, branch **main**, folder **/(root)**, then Save.
4. Wait for deployment and open `https://YOUR-USERNAME.github.io/ecoswap-adelaide/`. Replace YOUR-USERNAME with your GitHub username.
5. Test every page and the responsive navigation on mobile.

## Google Analytics 4 (GA4)
1. In [Google Analytics](https://analytics.google.com/), create an account/property and select **Australia/Adelaide** as the reporting time zone where appropriate.
2. Create a **Web** data stream for your published GitHub Pages URL. Copy the Measurement ID, formatted `G-XXXXXXXXXX`.
3. In the `<head>` of **each of the five HTML files**, find the commented GA4 snippet. Uncomment the two `<script>` tags and replace **both** `G-XXXXXXXXXX` occurrences with your real ID. Keep `window.ECOSWAP_GA4_ENABLED=true` in the activated snippet.
4. Commit and push changes. Reload the live site with analytics consent as appropriate and verify activity in **GA4 → Reports → Realtime**. Browser tracking protection or consent settings may affect results.
5. Test clicking **Browse demo items** and look for `browse_items_click` in Realtime or DebugView. Mark events as key events in GA4 only if relevant to the assessment.
6. Respect privacy and consent obligations. The demo contact form does not send personal data, but GA4 may collect browsing data once enabled. Add an appropriate privacy notice/consent mechanism before a public production launch.

**Important:** GA4 is a placeholder and is **disabled by default**. It cannot be verified until a real GA4 property is configured and the published site is visited.

## SEO and accessibility
- Unique page titles and descriptions; headings, semantic landmarks and meaningful links.
- Local Adelaide-focused keywords used naturally.
- Mobile layout, keyboard-accessible navigation, labels, status announcements and reduced-motion support.
- No canonical URLs yet because the final published URL is unknown. Once published, add a canonical URL to each page and update social sharing metadata.

## Academic integrity and AI use log
This package was AI-assisted. **Do not claim GitHub Copilot was used unless you actually use it.** In your assignment, document the real prompts, suggestions, manual edits, tests and screenshots from GitHub Copilot.

| Date | Tool | Task/prompt | AI output | Human review/change | Evidence |
|---|---|---|---|---|---|
| [fill] | GitHub Copilot | [actual prompt] | [actual suggestion] | [your modifications and tests] | [screenshot/commit] |

## Limitations
All products and prices are fictional. No backend, authentication, payments, messaging, database or working email delivery is included. Demo illustrations are inline SVG. Do not represent this prototype as an operating business.
