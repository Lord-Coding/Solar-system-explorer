# 🌍 Solar System Explorer

> An interactive tour of our solar system — **Pure CSS, No JavaScript**

[![Pure CSS](https://img.shields.io/badge/Pure-CSS-blue.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## ✨ Features

- **Planetary navigation** — click through all 8 planets + Pluto with smooth CSS transitions
- **Scientific data** — distance from Sun, diameter, mass, orbital period, surface temperature, atmospheric composition, and confirmed moon count for each planet
- **Fun facts** — one or two striking anecdotes per planet
- **Moon details** — key moons displayed in each planet's detail panel (Titan, Europa, Ganymede, Io, Triton…)
- **Source links** — links to NASA Solar System Exploration in every panel
- Pure CSS interactions — zero JavaScript, powered by radio inputs and the CSS `:checked` selector

## 📁 Project structure

```
Solar-system-explorer/
├── src/
│   ├── index.html      # Main HTML source
│   └── style.scss      # SCSS styles
├── dist/
│   ├── index.html      # Copied/served HTML
│   ├── style.css       # Compiled CSS
│   └── style.min.css   # Minified CSS (production)
├── .github/
│   └── workflows/
│       └── ci.yml      # GitHub Actions build check
├── package.json
├── vercel.json
└── README.md
```

## 🏗️ Build

```bash
# Install dependencies
npm install

# Build CSS
npm run build

# Watch SCSS for changes during development
npm run watch

# Build minified CSS for production
npm run build:prod
```

> `dist/index.html` is the `src/index.html` file served directly — no compilation step needed for HTML.

## 🛠️ Tech stack

| Layer | Technology |
|-------|------------|
| Markup | HTML5 |
| Styles | [SCSS / Sass](https://sass-lang.com/) |
| Output | HTML5 + CSS3 |

## ⚡ Performance

Planetary textures and images are currently loaded from third-party CDNs (NASA, gstatic, cosmosup). For production use, consider:

1. Download all textures locally into `assets/textures/`
2. Update the URLs in `src/style.scss` and `src/index.html`
3. Convert images to compressed **WebP** format to reduce bandwidth

This avoids broken images if external hosts change or go offline.

## 🎨 Credits

- Planet images & textures — [NASA](https://www.nasa.gov/) and various community sources
- Typography — [Montserrat](https://fonts.google.com/specimen/Montserrat) (Google Fonts)

## 🔗 Repository

[https://github.com/Lord-Coding/Solar-system-explorer](https://github.com/Lord-Coding/Solar-system-explorer)

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.
