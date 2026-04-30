# Factelys — Bibliothèque HTML partageable

Ce dossier est un site statique prêt à héberger. Il contient une interface en DA Factelys et tes documents HTML dans le dossier `documents/`.

## Structure

```
factelys_bibliotheque_site/
├── index.html
├── catalogue.js
├── documents/
│   ├── analyse-marche.html
│   ├── charte-graphique.html
│   ├── etude-brevo.html
│   ├── linkedin-kit.html
│   ├── forms-templates.html
│   └── offres-commerciales.html
└── README.md
```

## Hébergement conseillé

### Netlify avec compte gratuit
Crée un compte gratuit Netlify, puis glisse le dossier complet `factelys_bibliotheque_site` dans Netlify Drop depuis ton compte connecté. Le site restera en ligne.

### Vercel
Crée un nouveau projet, importe ce dossier comme projet statique, puis déploie.

### GitHub Pages
Mets tout le contenu du dossier dans un repository GitHub, active Pages sur la branche principale, et garde `index.html` à la racine.

### Hébergement classique
Envoie tout le contenu du dossier sur ton FTP, à la racine du site ou dans un sous-dossier.

## Ajouter un document

1. Mets ton nouveau fichier HTML dans `documents/`, par exemple :

```
documents/nouveau-document.html
```

2. Ouvre `catalogue.js` et ajoute une entrée :

```js
{
  "id": "nouveau-document",
  "num": "07",
  "title": "Nouveau document",
  "subtitle": "Description courte du document",
  "category": "Catégorie",
  "updated": "Avril 2026",
  "path": "documents/nouveau-document.html",
  "source": "nouveau-document.html"
}
```

3. Redéploie le dossier complet.

## Note

Les documents restent des fichiers HTML autonomes. Ils peuvent s'ouvrir dans le lecteur intégré ou dans un nouvel onglet.
