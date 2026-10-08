# TODO — Solar System Explorer

## 🔴 Critique (à corriger en priorité)

- [x] **Corriger l'état Git** — les fichiers actifs (`dist/`, `src/`) ne sont pas trackés ; supprimer l'ancien chemin `Solar System Explorer/` (avec espace) et restager les bons fichiers
- [x] **Créer un `package.json`** avec les scripts de build (`haml src/index.haml dist/index.html`, `sass src/style.scss dist/style.css`)
- [x] **Créer un `.gitignore`** (ignorer `node_modules/`, `.agents/`, fichiers OS, etc.)
- [x] **Supprimer les 2 `@debug`** dans `src/style.scss` (lignes 590–591)
- [x] **Corriger les `checked='checked'` multiples** dans `src/index.haml` — Mercury, Venus, Earth et Mars ont tous l'attribut en même temps ; garder uniquement Mercury comme sélection initiale

---

## 🟠 Élevé (qualité & contenu)

- [x] **Corriger ~50 fautes** `"solar systm"` → `"solar system"` dans `src/index.haml`
- [x] **Corriger 9 boutons tronqués** `"Read Mor"` → `"Read More"` dans `src/index.haml` — le split `Read Mor` + `%span e` est du markup intentionnel de kerning CSS ; le rendu produit déjà "Read More" correctement
- [x] **Rédiger le vrai contenu de Neptune** — remplacer le Lorem ipsum (ligne 226 de `src/index.haml`)
- [x] **Passer toutes les URLs d'images en HTTPS** — 8 URLs en `http://` risquent d'être bloquées en mixed-content
- [ ] **Héberger les images localement** ou sur un CDN stable (Cloudflare R2, BunnyCDN) — les ~40 images sur DeviantArt, gstatic, cosmosup, etc. peuvent disparaître sans préavis

---

## 🟡 Moyen (maintenabilité & accessibilité)

- [x] **Réduire les `!important`** dans `src/style.scss` (12+ occurrences) — revoir la spécificité CSS
- [x] **Supprimer Font Awesome** du `dist/index.html` s'il n'est pas utilisé, sinon l'exploiter pour des icônes
- [x] **Ajouter `<meta name="viewport">`** dans `src/index.haml`
- [x] **Ajouter des attributs `alt`** sur toutes les images dans les panneaux de planètes
- [x] **Ajouter des `aria-label`** sur les inputs radio et les éléments interactifs (accessibilité WCAG)
- [x] **Minifier le CSS** en production (`sass --style=compressed`) — `dist/style.css` fait 90KB non minifié
- [x] **Supprimer les commentaires de code déplacés** (ex. `# CloseUranus...lol`)

---

## 🟢 Faible (améliorations futures)

- [x] **Créer un `README.md`** — description du projet, aperçu visuel, instructions de build, crédits images/textures
- [x] **Configurer un CI minimal** (GitHub Actions) pour valider la compilation HAML/SCSS à chaque push
- [ ] **Optimiser le chargement des images** — lazy loading, ou ne charger les textures qu'à la sélection de la planète

---

## ✨ Fonctionnalités — Plus de détails sur les planètes

- [x] **Enrichir les fiches planètes** avec des données scientifiques supplémentaires :
  - Distance au Soleil (min/max/moyenne)
  - Diamètre et masse
  - Durée du jour et de l'année
  - Température de surface (min/max)
  - Nombre de lunes confirmées
  - Composition atmosphérique
  - Missions spatiales notables (Voyager, Cassini, New Horizons…)
- [x] **Ajouter une section "Faits insolites"** par planète (1 ou 2 anecdotes marquantes)
- [x] **Ajouter des liens vers des sources** (Wikipedia, NASA Solar System Exploration) dans chaque panneau
- [x] **Afficher les lunes dans le panneau de détail** — nom, taille, particularité pour les principales lunes (Titan, Europe, Ganymède, Io, Triton…)
- [ ] **Ajouter Pluton** en tant que planète naine avec une note sur son déclassement en 2006
- [ ] **Ajouter d'autres planètes naines** (Cérès, Éris, Makémaké, Hauméa) dans une section optionnelle
- [ ] **Comparateur de tailles** — un visuel CSS comparant la taille des planètes entre elles et par rapport au Soleil
- [ ] **Timeline des découvertes** — frise chronologique des découvertes de chaque planète

---

*Dernière mise à jour : 07/10/2026*
