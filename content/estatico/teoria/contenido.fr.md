---
title: "Ajouter du contenu"
date: 2021-11-07T20:44:12+01:00
draft: false
weight: 11
---
**Ajouter du contenu aux pages**
> Pour ajouter du contenu, vous devez générer des pages de texte au format **markdown**
```
Création de pages de contenu
```
**Il est important de bien établir l'organisation du contenu**
+ Créer des répertoires de chapitres ou de sections. Vous pouvez inclure un fichier _index.md
+ Créez des fichiers de contenu avec la commande `hugo new section_name / file_name.md`
+ Les fichiers sont créés dans le dossier ** content ** du répertoire racine du site
+ Les sections ou chapitres ont un contenu par défaut spécifié dans `archetypes/chapitre.md`
+ Les fichiers ont un contenu par défaut spécifié dans `archetypes / default.md`
+ Chaque fichier créé a le **front matter** au début, enfermé entre deux blocs de 3 lignes - - -
+ **Les taxonomies** vous permettent de classer le contenu. Par défaut, hugo ajoute les taxonomies **categories** et **tags**

