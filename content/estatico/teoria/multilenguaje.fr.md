---
title: "Multilingue"
date: 2021-11-07T20:50:09+01:00
draft: false
weight: 14
---
**Définir différentes langues dans hugo**
**1. Modifier config.toml**
![captura_idiomas](/images/captura_idiomas.png)
***
**2. Vous pouvez définir une langue par défaut**
![captura_pordefecto](/images/captura_pordefecto.png)
***
**3. Changer la page par défaut**
+ Vous devez définir le contenu de la page par défaut dans les langues
+ Dans **learn**, s'il n'y a pas de contenu dans "content", ce contenu est dans le fichier **index.html**, situé dans `themes / learn / layouts`
+ Ce modèle est préparé pour l'anglais et le français, vous devez donc ajouter une structure de contrôle pour inclure une autre langue
***
**4. Modification des valeurs via des variables**
+ Les mots peuvent être spécifiés pour être traduits
+ Dans **i18n**, les 2 premières lettres des fichiers identifient la langue
+ Ces fichiers sont traduits et le système obtient la valeur du fichier, en utilisant la fonction de traduction de hugo
![captura_traduccion](/images/captura_traduccion.png)
***
**5. Menus en plusieurs langues**
+ Définir dans config.toml :
```
   [Languages]
   [Languages.fr]
   ...
   [[Languages.fr.menu.shortcuts]]
   ```
***
**6. Ajout de pages traduites**
> Une façon de préciser les traductions est de nommer chaque fichier correspondant à une page référençant les langues
```
fichier.es.md
fichier.en.md
fichier.fr.md
```
+ Dans config.toml, indiquez, avec la variable **ContentDir**, le répertoire où se trouvent les fichiers traduits dans la langue :
```
   [Languages]
   [Languages.fr]
   ...
      ContentDir = "content"
```

