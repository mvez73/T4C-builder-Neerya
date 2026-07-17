![GitHub deployments](https://img.shields.io/github/deployments/mvez73/T4C-builder-Neerya/github-pages) ![GitHub License](https://img.shields.io/github/license/mvez73/T4C-builder-Neerya) ![W3C Validation](https://img.shields.io/w3c-validation/html?targetUrl=https%3A%2F%2Fmvez73.github.io%2FT4C-builder-Neerya%2F) [![Live Demo](https://img.shields.io/badge/Live%20Demo-View%20Site-brightgreen?logo=googlechrome&logoColor=white)](https://mvez73.github.io/T4C-builder-Neerya/)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)


# T4C Neerya - Créateur de personnage

Outil statique (page unique) pour **T4C-Neerya**, un serveur privé de The 4th Coming. On entre les statistiques de son personnage (Force, Endurance, Dextérité, Sagesse, Intelligence) et sa Renaissance, et l'outil calcule le niveau du personnage puis filtre une catégorie d'objets/sorts pour ne montrer que ce qui est utilisable actuellement.

🔗 [Voir le site](https://mvez73.github.io/T4C-builder-Neerya/) · [Changelog](CHANGELOG.md)

## Fonctionnalités

- Calcul du niveau de personnage selon la Renaissance (Humain, Renaissance 1, Renaissance 2).
- Bonus de statistiques liés aux quêtes (Purification des ruines d'Anwynn, Quêtes Ebon Hold — niveau 75+ requis).
- Filtrage par catégorie : sorts, compétences, arcs, armes de mêlée, robes, capes, armures, bijoux.
- Aucune inscription, aucun serveur : tout tourne dans le navigateur.

## Lancer le projet localement

Le site charge ses données via `fetch('*.json')`, ce qui échoue en ouvrant directement le fichier (`file://`) à cause des restrictions CORS. Il faut donc servir les fichiers via un petit serveur HTTP :

```bash
python -m http.server 8000
```

Puis ouvrir `http://localhost:8000/index.html`. Lancer la commande depuis la racine du dépôt pour que les chemins des fichiers JSON fonctionnent. Après une modification, faire un rechargement forcé (Ctrl+F5) pour éviter le cache du navigateur.

Il n'y a pas de build, de linter ni de tests automatisés dans ce projet.

## Structure du projet

- `index.html` — tout le site : structure, styles (`<style>`) et logique (`<script>`) inline.
- `*.json` — un fichier par catégorie d'objets/sorts, chargé à la demande.
- `CHANGELOG.md` — historique des changements par version Beta.

## Versionnage

Un badge `Beta 0.xxx` apparaît dans l'en-tête, à côté de "CRÉATEUR DE PERSONNAGE". Ce numéro est incrémenté à chaque changement et documenté dans le [Changelog](CHANGELOG.md).

## Contribuer

Ce projet est maintenu de façon informelle pour la communauté T4C-Neerya. Pour signaler une erreur de donnée (statistiques, prix, description manquante) ou une suggestion, ouvrir une [issue](https://github.com/mvez73/T4C-builder-Neerya/issues) sur GitHub.
