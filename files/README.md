# POLYSCAN — Polymarket Dashboard

> A minimalist, dark-themed prediction market tracker built with vanilla HTML/CSS/JS.  
> No framework. No dependencies. Just open the file and go.

![Dashboard Preview](https://img.shields.io/badge/status-live-39ff14?style=flat-square&labelColor=0d1117)
![Tech](https://img.shields.io/badge/stack-HTML%20%2F%20CSS%20%2F%20JS-00e5ff?style=flat-square&labelColor=0d1117)
![License](https://img.shields.io/badge/license-MIT-ff4d6d?style=flat-square&labelColor=0d1117)

---

## Features

- **Live data** — fetches the top 100 active markets from Polymarket's Gamma API
- **YES / NO probability bars** — animated, color-coded (green / red)
- **Stats bar** — total markets, active count, average YES probability, high-confidence count
- **Filters** — High confidence (>80%) and Close call (40–60%) to spot opportunities
- **Full-text search** — filter markets by keyword in real time
- **Pagination** — 12 markets per page
- **Click-through** — click any card to open the market directly on Polymarket

---

## Usage

### Option 1 — Open locally
Just download `index.html` and open it in your browser.

> ⚠️ Some browsers block CORS requests from `file://`. If data doesn't load, use Option 2.

### Option 2 — Local server (recommended)
```bash
# Python
python3 -m http.server 8080

# Node
npx serve .
```
Then open `http://localhost:8080`

### Option 3 — GitHub Pages
Fork this repo, go to **Settings → Pages → Source: main / root** and your dashboard will be live at:
```
https://<your-username>.github.io/polymarket-dashboard
```

---

## API

Data is sourced from Polymarket's public API — no API key required.

| Endpoint | Description |
|---|---|
| `gamma-api.polymarket.com/markets` | Market metadata, questions, probabilities, volume |

---

## Stack

- **HTML5 / CSS3 / Vanilla JS** — zero build step, zero dependencies
- **Google Fonts** — Syne + Space Mono
- **Polymarket Gamma API** — public, unauthenticated

---

## Roadmap

- [ ] Portfolio tracker — input your positions and track P&L
- [ ] Category filtering (crypto, politics, sports...)
- [ ] Sort by volume / end date / probability
- [ ] Price history chart per market
- [ ] Alerts for markets crossing probability thresholds

---

## Author

**Kilian Mongey** — [@Bitkilou](https://github.com/Bitkilou) · [@Tumbleur](https://twitter.com/Tumbleur)

Professional contortionist at Cirque du Soleil. Bitcoin & sound money advocate.  
Building tools at the intersection of prediction markets and open-source finance.

---

## License

MIT — free to use, modify, and share.
