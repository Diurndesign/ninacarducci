# Nina Carducci — Optimisation SEO, performance & accessibilité

Site vitrine de **Nina Carducci**, photographe professionnelle à Bordeaux.
Ce dépôt contient la version **optimisée** du site : amélioration du référencement
naturel (SEO), des performances et de l'accessibilité, **sans modifier le design**.

🔗 **Site en ligne :** https://diurndesign.github.io/ninacarducci/

---

## 📊 Résultats des audits (après optimisation)

| Audit | Résultat |
|---|---|
| **Lighthouse — Performance** | 97 / 100 |
| **Lighthouse — Accessibilité** | 100 / 100 |
| **Lighthouse — Bonnes pratiques** | 100 / 100 |
| **Lighthouse — SEO** | 100 / 100 |
| **WAVE (accessibilité)** | 0 erreur · 0 alerte · score AIM 10/10 |
| **Google Rich Results** | ✅ 1 élément valide (`LocalBusiness`) |

Métriques clés : **FCP 0,5 s · LCP 1,1 s · CLS conforme**.

---

## 🔍 Améliorations SEO

### Balises et métadonnées
- **`<title>`** optimisé avec le métier **et** la ville : *« Nina Carducci — Photographe professionnelle à Bordeaux »*.
- **Meta description** ciblée avec les mots-clés et la localisation.
- **`lang="fr"`** sur la balise `<html>` (langue du contenu).
- **Balise canonical** pour éviter le contenu dupliqué.
- **Open Graph** et **Twitter Card** complets (aperçu riche lors des partages sur les réseaux sociaux).

### Données structurées (Schema.org / JSON-LD)
- Ajout d'un bloc **`LocalBusiness`** : nom, adresse, téléphone, coordonnées GPS et horaires.
- Corrections de 3 erreurs qui empêchaient la lecture par Google :
  - `@type` invalide `ProfessionnalService` → **`LocalBusiness`** ;
  - propriété `geocoordinates` (ignorée) → **`geo`** ;
  - `og:image:type` corrigé (`image/avif`).
- Rend le site **éligible aux résultats enrichis** (Rich Snippet).

### Contenu et sémantique
- Texte **« À propos » enrichi** avec les mots-clés de la niche (mariage, portrait, concert, événement d'entreprise, séance photo, retouche), en conservant le ton d'origine.
- Attributs **`alt`** descriptifs sur toutes les images (référencement Google Images + accessibilité).
- Hiérarchie de titres cohérente (un seul `<h1>`, des `<h2>`/`<h3>` structurés).

### Référencement local
- Ville **Bordeaux** intégrée dans le title, la description et le contenu.
- Adresse structurée (`LocalBusiness`) localisée à Bordeaux.
- **Cohérence géographique** rétablie : « Île-de-France » → **« région bordelaise »** sur tout le site.

---

## ⚡ Améliorations de performance

> La vitesse est un critère de classement de Google (Core Web Vitals).

- **Images : ~88 Mo → 1,2 Mo (−98 %)** — redimensionnées à leur taille réelle d'affichage et recompressées en **AVIF** (carrousel) et **WebP** (galerie, portraits).
- **Image LCP** (1re du carrousel) **préchargée** (`preload`) et prioritaire (`fetchpriority="high"`).
- **Google Fonts** en chargement **non-bloquant**.
- **Scripts** déplacés en bas de page + attribut **`defer`**.
- **CSS/JS minifiés** (`style.min.css`, `scripts.min.js`, `maugallery.min.js`).
- Suppression de **~1,6 Mo** de fichiers Bootstrap inutiles (sources et *source maps*).
- **Stabilité visuelle (CLS)** : attributs `width`/`height` sur toutes les images + `img { height: auto }`.

---

## ♿ Améliorations d'accessibilité

- **Balises sémantiques** (landmarks) : `<header>`, `<nav>`, `<main>`.
- **Labels de formulaire** liés aux champs (`for` / `id`).
- **Textes alternatifs** (`alt`) sur toutes les images.
- **Contraste** conforme (boutons de filtre + textes cachés des flèches du carrousel).
- Attributs **`aria-label`** sur les boutons du carrousel et le lien Instagram.

---

## 🗂️ Structure du projet

```
.
├── index.html              # Page principale (optimisée)
├── assets/
│   ├── bootstrap/          # Bootstrap (fichiers minifiés utiles uniquement)
│   ├── images/             # Images optimisées (AVIF / WebP)
│   ├── style.min.css       # Styles du site (minifiés)
│   ├── scripts.min.js      # Initialisation de la galerie
│   └── maugallery.min.js   # Librairie galerie / lightbox
└── README.md
```

---

## 🛠️ Outils utilisés

- **Google Lighthouse** — performance, accessibilité, bonnes pratiques, SEO
- **Google Rich Results Test** — validation des données structurées
- **Extension WAVE (WebAIM)** — accessibilité

> Astuce : lancer les audits Lighthouse en **navigation privée** pour éviter que les
> extensions du navigateur ne faussent le rapport.

---

## 👤 Auteur

Optimisation réalisée par **Jeremy Bendenoun**.
