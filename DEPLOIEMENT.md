# Mise en ligne — Liens Edouard Richard

Page de liens (type Linktree) d'Edouard Richard, compagnon du portfolio [erchd.photos](https://edouardrchd.github.io/erchd.photos/).

| Fichier | Rôle |
|---|---|
| `index.html` | La page entière : HTML statique, styles inline, JavaScript natif en fin de page. Aucune dépendance : pas de React, pas de runtime de design, pas de CDN, pas de build. |
| `fonts/` | Polices auto-hébergées (sous-ensemble latin) : Antonio, Archivo, Bodoni Moda, IBM Plex Mono. Licence SIL OFL 1.1. |

## Déploiement (GitHub Pages)

Settings → Pages → Source : `Deploy from a branch`, branche `main`, dossier `/ (root)`.
URL : `https://edouardrchd.github.io/erchd.links/`

## Modifier un lien

Chaque lien est un bloc `<a data-row …>` dans `index.html` :
- `href` : la destination réelle ;
- `data-target` : le texte affiché en bas de page au survol ;
- le numéro, le titre (Bodoni) et la ligne de détail (mono) sont en texte brut.

Pour ajouter un lien, dupliquer un bloc, renuméroter, et décaler le délai d'animation (`both 1820ms`, `1900ms`… +80 ms par ligne).

## À compléter

- **Facebook** : `href` pointe encore sur `https://facebook.com/` (page d'accueil) alors que le survol affiche `facebook.com/edouardrichardphoto`. Mettre la vraie URL de la page, ou supprimer la ligne.
- `og:image` réutilise l'image du portfolio.
