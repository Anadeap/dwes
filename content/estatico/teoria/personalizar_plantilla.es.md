---
title: "Personalizar plantilla"
date: 2021-11-07T20:48:53+01:00
draft: false
weight: 13
--- 
## Partes de una plantilla  
**1. LOGO**  
+ **logo.html** está ubicado en themes/layouts/partials  
+ Para personalizar el logo, copiar el fichero en mi_sitio/layouts/partials  
+ Crear en static una carpeta - images - y dentro pegar un logo.png  
+ Referenciarlo en logo.html
![captura_logo](/images/captura_logo.png)
***
**2. MENÚ**  
+ En la plantilla **learn**, el menú está ubicado en la parte izquierda.  
+ Para añadir/modificar, hay que especificarlo en **config.toml**, añadiendo los elementos **[[menu.shortcuts]]**  
![captura_menu_shortcuts](/images/captura_menu_shortcuts.png)  
+ El **título** del menú se establece en **/i18n/es.toml** para el idioma español  
![captura_titulo_menu](/images/captura_titulo_menu.png)
***
**3. ESTILO**
+ **learn** tiene 3 estilos de colores diferentes
+ Para utilizarlos, hay que establecer el valor en la variable **themeVariant** en el fichero **config.toml**
+ Los valores permitidos son **red, green, blue**
+ También se pueden crear **ficheros css** y cargarlos.  Por ejemplo, para establecer otro color de fondo del menú distinto a los colores por defecto:  
> Copiar `themes/learn/static/css/theme-blue.css` en un fichero **theme-dwes.css** ubicado en `static/css`  
Establecer **themeVariant = "dwes"**
***
**4. BOTÓN DE BÚSQUEDA**
+ Se puede modificar desde theme-dwes.css
**5. HOME**
+ Se modifica en **config.toml**, modificando los parámetros dentro de una sección de lenguaje
***
**5. FOOTER**
+ Para modificarlo, copiar **menu-footer.html** en layouts/partials

