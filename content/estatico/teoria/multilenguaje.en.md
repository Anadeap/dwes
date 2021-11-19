---
title: "Multilanguage"
date: 2021-11-07T20:50:09+01:00
draft: false
weight: 14
---
**Set different languages ​​in hugo**
**1. Modify config.toml** 
![captura_idiomas](/images/captura_idiomas.png)
***
**2. You can set a default language**
![captura_pordefecto](/images/captura_pordefecto.png)
***
**3. Changing the default page**
+ You have to set the content of the page by default in the languages
+ In **learn**, if there is no content in "content", this content is in the **index.html** file, located in `themes / learn / layouts`
+ This template is prepared for English and French, so you have to add a control structure to include another language
***
**4. Changing values ​​through variables**
+ Words can be specified to be translated
+ In **i18n**, the first 2 letters of the files identify the language
+ These files translate and the system gets the value of the file, using hugo's translation function
![captura_traduccion](/images/captura_traduccion.png)
***
 **5. Menus in several languages ​​**
+ Set in config.toml:
```
   [Languages]
   [Languages.en]
   ...
   [[Languages.en.menu.shortcuts]]
   ```
***
** 6. Adding translated pages**
> One way to specify the translations is to name each file corresponding to a page referencing the languages
```
file.es.md
file.en.md
file.fr.md
```
+ In config.toml, indicate, with the variable **contentDir**, the directory where the files translated into the language are located:
```
   [Languages]
   [Languages.en]
   ...
      ContentDir = "content"
```

