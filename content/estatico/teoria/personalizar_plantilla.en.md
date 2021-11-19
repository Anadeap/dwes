---
title: "Customize template"
date: 2021-11-07T20:48:53+01:00
draft: false
weight: 13
--- 
## Parts of a template  
**1. LOGO**  
+ **logo.html** is located in themes/layouts/partials  
+ To customize the logo, copy the file in my_site/layouts/partials  
+ Create in static a folder - images - and inside paste a logo.png  
+ Reference it in logo.html
![captura_logo](/images/captura_logo.png)
***
**2. MENU**  
+ In the layout **learn**, the menu is located in the left side 
+ To add / modify, you have to specify it in **config.toml**, adding the elements **[[menu.shortcuts]]**  
![captura_menu_shortcuts](/images/captura_menu_shortcuts.png)  
+  The **title** of the menu is set in **/i18n/en.toml** for the English language   

![captura_title_menu](/images/captura_title_menu.png)
***
**3. STYLE**
+ **learn** has 3 different color styles
+ To use them, you have to set the value in the variable **themeVariant** in the file **config.toml**
+ Allowed values ​​are **red, green, blue**
+ You can also create **css files** and load them. For example, to set a menu background color other than the default colors:  
> Copy `themes/learn/static/css/theme-blue.css` in a file **theme-dwes.css** located in `static/css`  
Establish **themeVariant = "dwes"**
***
**4. SEARCH BUTTON**
+ It can be modified from theme-dwes.css
**5. HOME**
+ It is modified in **config.toml**, modifying the parameters within a language section
***
**5. FOOTER**
+ To modify it, copy **menu-footer.html** in layouts / partials

