---
title: "Personnaliser la disposition"
date: 2021-11-07T20:48:53+01:00
draft: false
weight: 13
---
## Parties d'un  modéle 
**1. LOGO**  
+ **logo.html** se trouve dans themes/layouts/partials  
+ Pour personnaliser le logo, copiez le fichier dans mon_site/layouts/partials
+ Créer en statique un dossier - images - et à l'intérieur coller un logo.png
+ Référencez-le dans logo.html
![captura_logo](/images/captura_logo.png)
***
**2. MENU**
+ Dans la mise en page **learn**, le menu est situé sur le côté gauche
+ Pour ajouter/modifier, il faut le préciser dans **config.toml**, en ajoutant les éléments **[[menu.shortcuts]]**
![captura_menu_shortcuts](/images/captura_menu_shortcuts.png)  
+  The **titre** du menu est défini en **/i18n/fr.toml** pour la langue francais  

![captura_titre_menu](/images/captura_titre_menu.png)
***
**3. STYLE**
+ **learn** a 3 styles de couleurs différents
+ Pour les utiliser, vous devez définir la valeur dans la variable **themeVariant** dans le fichier **config.toml**
+ Les valeurs autorisées sont **red, green, blue**
+ Vous pouvez également créer des **fichiers css** et les charger. Par exemple, pour définir une couleur d'arrière-plan de menu autre que les couleurs par défaut :
> Copier `themes/learn/static/css/theme-blue.css` dans un fichier **theme-dwes.css** situé dans `static/css`  
L'estable **themeVariant = "dwes"**
***
**4. BOUTON DE SEARCH**
+ Il peut être modifié à partir de theme-dwes.css
**5. HOME**
+ Il est modifié dans **config.toml**, en modifiant les paramètres au sein d'une section de langue
***
**5. FOOTER**
+ Pour le modifier, copiez **menu-footer.html** dans layouts / partials

