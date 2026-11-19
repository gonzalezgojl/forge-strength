# French 360

Application mobile-first pour travailler le français 60 minutes par jour.

## Fonctionnalités

- Session quotidienne : vocabulaire (10 min), grammaire (15 min), écoute (15 min), expression orale (10 min) et révision (10 min).
- Parcours guidé de 12 semaines, du français quotidien au français professionnel aéronautique.
- Cartes de vocabulaire espagnol → français, avec un filtre Vie quotidienne / Aéronautique.
- Dialogues pratiques pour l'hôtel, l'aéroport et la maintenance.
- Mini-quiz et lecture des phrases avec la synthèse vocale disponible sur l'appareil.
- Progression locale : activités cochées, cartes maîtrisées et minutes étudiées.
- PWA avec cache hors ligne et installation sur l'écran d'accueil.

## Déployer avec GitHub Pages

Dans le dépôt, ouvrir **Settings → Pages**, choisir **Deploy from a branch**, sélectionner `main` et `/ (root)`, puis enregistrer.
La page sera disponible à :

`https://gonzalezgojl.github.io/forge-strength/french-360/`

## Installer sur iPhone

1. Ouvrir l'adresse ci-dessus dans Safari.
2. Toucher **Partager**.
3. Choisir **Ajouter a la pantalla de inicio / Añadir a pantalla de inicio**.
4. Confirmer **Ajouter**. L'icône French 360 apparaîtra sur l'écran d'accueil.

## Données et confidentialité

La progression est enregistrée dans le stockage local du navigateur. Cette première version ne synchronise pas encore les données entre appareils et ne nécessite aucun compte.

## Structure

- `index.html` — application et interface.
- `manifest.webmanifest` — configuration PWA.
- `sw.js` — cache hors ligne.
- `icon.svg` — icône de l'application.
