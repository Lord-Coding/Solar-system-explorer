# 🌍 Solar System Explorer

> An interactive tour of our solar system — **Pure CSS, No JavaScript**

[![Pure CSS](https://img.shields.io/badge/Pure-CSS-blue.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## ✨ Features

- **Planetary navigation** — click through all 8 planets with smooth CSS transitions
- **Scientific data** — distance from Sun, diameter, mass, orbital period, surface temperature, atmospheric composition, and confirmed moon count for each planet
- **Fun facts** — one or two striking anecdotes per planet
- **Moon details** — key moons displayed in each planet's detail panel (Titan, Europa, Ganymède, Io, Triton…)
- **Source links** — links to Wikipedia and NASA Solar System Exploration in every panel
- Pure CSS interactions — zero JavaScript, powered by radio inputs and the CSS `:checked` selector

## 🏗️ Build

```bash
# Install Sass
npm install

# Build HTML (requires haml gem)
npm run build:html

# Build CSS
npm run build:css

# Build all
npm run build

# Build minified CSS for production
npm run build:prod
```

## 🛠️ Tech stack

| Layer | Technology |
|-------|------------|
| Templating | [HAML](https://haml.info/) |
| Styles | [SCSS / Sass](https://sass-lang.com/) |
| Output | HTML5 + CSS3 |

## ⚡ Performance

Planetary textures and images are currently loaded from third-party CDNs (NASA, gstatic, cosmosup, DeviantArt). For production use, consider:

1. Download all textures locally into `assets/textures/`
2. Update the URLs in `src/style.scss` and `src/index.haml`
3. Convert images to compressed **WebP** format to reduce bandwidth

This avoids broken images if external hosts change or go offline.

## 🎨 Credits

- Planet images & textures — [NASA](https://www.nasa.gov/) and various community sources
- Typography — [Montserrat](https://fonts.google.com/specimen/Montserrat) (Google Fonts)
- Icons — [Font Awesome](https://fontawesome.com/)

## 🔗 Repository

[https://github.com/Lord-Coding/Solar-system-explorer](https://github.com/Lord-Coding/Solar-system-explorer)

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.
