# Suivi des temps de natation

Site statique de suivi des performances de natation : records personnels, progression, meilleurs temps par âge et historique des compétitions.

## Fichiers

- `index.html` : le site (affichage et calculs). Pas besoin d'y toucher.
- `donnees.js` : les nageurs et leurs temps. **C'est le seul fichier à mettre à jour.**

## Ajouter un temps

Dans `donnees.js`, copier une ligne de `PERFORMANCES`, la coller à la fin de la liste et changer les valeurs :

```js
{ nageur: "luka", date: "2026-12-06", epreuve: "100 Dos", temps: "1:37.80", points: 310, bassin: 25, lieu: "THIONVILLE", niveau: "REG" },
```

L'âge, la saison, les records et la progression sont recalculés automatiquement.

## Mise en ligne avec GitHub Pages

1. Créer un dépôt et y déposer `index.html` et `donnees.js`.
2. Dans **Settings > Pages**, choisir la branche `main` et le dossier `/ (root)`.
3. Le site est disponible à l'adresse `https://<identifiant>.github.io/<nom-du-depot>/`.

Le site fonctionne aussi en local, en ouvrant `index.html` dans un navigateur.

## Ajouter un autre nageur

Ajouter une ligne dans `NAGEURS` (avec un `id` unique), puis ses temps dans `PERFORMANCES` avec ce même `id`. Un menu de choix du nageur apparaît alors automatiquement en haut du site.
