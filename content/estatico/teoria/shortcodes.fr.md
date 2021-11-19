---
title: "Shortcodes"
date: 2021-11-07T20:45:32+01:00
draft: false
weight: 12
---
### EXEMPLES DE SHORTCODES
> Un **shortcode** est un extrait de code html qui sera rendu dans un fichier md lorsque le système chargera ou affichera la page de contenu
1. **Buttons**  
_Bouton qui renvoie au site Web d'Hugo_   
{{% button href="https://gohugo.io/" icon="fas fa-download" %}}Le site d'hugo{{% /button %}}

***
2. **Attachments - pages de téléchargement**
| Pages | Emplacement des pièces jointes |
| ------ | ---------------------- |
| md | dans le répertoire avec le même nom de page et se terminant par .files |
| annuaire | dans un répertoire de fichiers imbriqués |    

{{%attachments title="Attachments" style="orange" /%}} 
***
3. **Raccourcir un texte avec Lire la suite...** Cliquez sur le texte pour développer
{{%expand "Hugo est l'un des générateurs de sites statiques open source les plus populaires." %}} Avec sa vitesse et sa flexibilité incroyables, Hugo rend la création de sites Web amusante à nouveau. {{% / expand%}}
***
4. **Textes surlignés**  
Nouvelles
{{% notice note %}}
Nouvelles
{{% /notice %}}
Informations
{{% notice tip %}}
Informations
{{% /notice %}}
Avis
{{% notice warning %}}
Avis
{{% /notice %}}
***
5. **Tabs de différents éléments**  
Très utile pour fournir des extraits de code pour plusieurs langues ou fournir des paramètres dans différents formats 
{{< tabs groupId="config" >}}
{{% tab name="json" %}}
```json
{
  "Hello": "World"
}
```
{{% /tab %}}
{{% tab name="XML" %}}
```xml
<Hello>World</Hello>
```
{{% /tab %}}
{{% tab name="properties" %}}
```properties
Hello = World
```
{{% /tab %}}
{{< /tabs >}}
***
6. **Lien vers une vidéo youtube**  
{{< youtube 6H0jLIKe0uw >}}

