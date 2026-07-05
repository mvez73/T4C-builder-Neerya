# Changelog

Toutes les modifications notables de ce projet sont documentées ici.

## Beta 0.041
- Le champ "Recherche" adopte maintenant le même style visuel (fond sombre, bordure bleue, focus) que les autres champs du formulaire, au lieu d'un fond blanc par défaut.

## Beta 0.040
- Ajout d'un champ "Recherche" au-dessus du tableau permettant de filtrer par n'importe quelle information (nom, conditions, description, obtention, bonus, etc.), avec support des opérateurs ET (espace) et OU (virgule).

## Beta 0.039
- Audit complet des fichiers de données (`arcs`, `armures`, `bijoux`, `mêlée`, `robes`, `sorts`, `compétences`, `capes`) contre leurs sources wiki : restauration de mise en forme (`<strong>`/`<em>`) et de liens de quête manquants, correction de valeurs de colonnes et de champs "Obtention" tronqués (matériaux d'amélioration, clauses de sorts, formules).

## Beta 0.038
- Le lien "Changelog" de l'en-tête pointe maintenant vers `CHANGELOG.md` au lieu de l'historique des commits.

## Beta 0.037
- Amélioration de l'affichage responsive sur petits écrans (mobile).
- Ajout d'une règle dans `.gitignore` pour exclure les fichiers de sauvegarde d'`index.html`.

## Beta 0.036
- Ajout du README.md et du présent CHANGELOG.md.

## Beta 0.035
- Ajout de liens "Projet GitHub" et "Changelog" dans l'en-tête.
- Le champ "Quêtes Ebon Hold" affiche un placeholder ("Niveau 75+ requis") au lieu d'un label qui débordait, quand la condition de niveau n'est pas remplie.

## Beta 0.034
- Le label du champ Ebon Hold précise la condition de niveau 75+.

## Beta 0.033
- Le texte en gras (`<strong>`) dans les colonnes Informations/Obtention est maintenant mis en évidence avec une couleur distincte, en plus du gras, pour être plus visible dans le tableau.

## Beta 0.032
- La quête Ebon Hold est désormais désactivée et réinitialisée automatiquement si le niveau du personnage (calculé sans son propre bonus) est inférieur à 75.

## Beta 0.031
- Reconstruction complète des données `melees.json` à partir des fichiers sources du wiki : suppression de 69 doublons, complétion des descriptions tronquées (colonnes Informations/Obtention), correction de la vitesse d'attaque des armes paladin (valeur décimale mal convertie), et ajout de la donnée "Cap dex" manquante pour la classe ante-paladin.

## Beta 0.030 et antérieures
- Mise en place initiale du site : filtrage des objets/sorts par statistiques et niveau, calcul du niveau de personnage selon la Renaissance, thème sombre responsive.
- Ajout des bonus de statistiques liés aux quêtes (Purification des ruines d'Anwynn, Quêtes Ebon Hold) dans le calcul du niveau.
- Ajout des données arcs, mêlée, sorts, compétences et liens vers le wiki.
