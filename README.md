# GEO//INTEL — Country Explorer [The project is still under development.]

> A dark sci-fi geo-intelligence dashboard for exploring every nation on Earth.

![GEO//INTEL](https://img.shields.io/badge/STATUS-LIVE-00ff6a?style=for-the-badge&labelColor=020c06)
![Version](https://img.shields.io/badge/VERSION-2.4.1-00cc55?style=for-the-badge&labelColor=020c06)
![API](https://img.shields.io/badge/API-REST_COUNTRIES-ffaa00?style=for-the-badge&labelColor=020c06)
![License](https://img.shields.io/badge/LICENSE-MIT-5aaf75?style=for-the-badge&labelColor=020c06)

---

## Overview

GEO//INTEL is a single-file, zero-dependency country explorer built with pure HTML, CSS, and JavaScript. Styled as a classified government intelligence terminal, it pulls live data from the REST Countries API to display detailed intel on all 195 sovereign nations — from population density to bordering nations, satellite maps, currencies, and more.

---

## Features

- **195 Nations Indexed** — full global database loaded on startup
- **Instant Search** — query by country name, capital city, or country code (CCA2/CCA3)
- **Region Filters** — filter by Asia, Europe, Americas, Africa, or Oceania
- **Deep Country Intel** — each nation card shows:
  - Flag, official name, native name
  - Capital, region, subregion
  - GPS coordinates, area, population, population density
  - Timezone, calling code, top-level domain
  - Languages and currencies
  - Status badges (Independent / UN Member / Territory)
  - Bordering nations (clickable — jumps directly to that country)
  - Embedded satellite map with dark filter
- **Live UTC Clock** — real-time clock in the header
- **Sci-Fi UI Effects** — animated scanline beam, CRT overlay, glitch title animation, pulsing status dot

---

## Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Structure |
| CSS3 | Styling, animations, scanline effects, responsive layout |
| Vanilla JavaScript | Logic, API calls, filtering, DOM rendering |
| [REST Countries API](https://restcountries.com/) | Country data (free, no key required) |
| [OpenStreetMap](https://www.openstreetmap.org/) | Embedded maps (free, no key required) |
| [Google Fonts](https://fonts.google.com/) | Orbitron · Share Tech Mono · Rajdhani |

> No npm. No build tools. No dependencies. Just open the file and run.

---

## Getting Started

```bash
git clone https://github.com/your-username/geo-intel.git
cd geo-intel
open country-explorer.html
```

Or simply drop `country-explorer.html` into any browser — it works offline after the first load (fonts and API aside).

---

## API Reference

Powered entirely by the free [REST Countries API](https://restcountries.com/) — no API key required.

| Endpoint | Usage |
|---|---|
| `GET /v3.1/all?fields=...` | Fetch all countries with selected fields on startup |

Fields requested: `name, cca2, cca3, flags, region, subregion, capital, population, area, languages, currencies, borders, timezones, continents, independent, unMember, latlng, tld, idd`

Maps are rendered via embedded [OpenStreetMap](https://www.openstreetmap.org/export/) iframes — no key needed.

---

## Project Structure

```
geo-intel/
└── country-explorer.html    # Entire app — HTML + CSS + JS in one file
```

---

## Design System

GEO//INTEL uses a custom dark terminal design language:

| Token | Value |
|---|---|
| Background | `#020c06` (near-black green-tinted) |
| Accent / Glow | `#00ff6a` (terminal green) |
| Amber | `#ffaa00` (warning / UN badge) |
| Red | `#ff3344` (alert / territory badge) |
| Display Font | Orbitron (headings, logo) |
| Mono Font | Share Tech Mono (data readouts) |
| Body Font | Rajdhani (labels, UI text) |

**Visual effects include:** animated scanline sweep beam, CRT scanline overlay, title glitch animation, pulsing live indicator dot, and hover glow states throughout.

---

## Screenshots

| Idle State | Country Detail |
|---|---|
| Grid animation + global stats | Flag, data grid, map, borders |

---

## Known Limitations

- Requires an internet connection to fetch country data and render maps
- Some countries may have missing YouTube or map coordinates in the source API
- OpenStreetMap embed uses a dark CSS filter — may look slightly off on some browsers
- No offline/PWA support yet

---

## Roadmap

- [ ] Favourites / bookmark countries
- [ ] Compare two nations side by side
- [ ] Population and area bar charts
- [ ] Dark/light theme toggle
- [ ] PWA support for offline use
- [ ] Export country data as JSON or CSV

---

## Contributing

Pull requests are welcome. For major changes, open an issue first to discuss what you'd like to change.

---

## License

MIT — free to use, modify, and distribute.

---

<div align="center">

```
GEO//INTEL v2.4.1 — GLOBAL INTELLIGENCE NETWORK ACTIVE
195 SOVEREIGN NATIONS INDEXED — ALL SYSTEMS NOMINAL
```

</div>
