---
title: "Añadir contenido"
date: 2021-11-07T20:44:12+01:00
draft: false
weight: 11
---
**Añadir contenido a las páginas**  
> Para añadir contenido hay que generar páginas de texto con formato **markdown**  
```
Creando páginas de contenido
```
**Es importante establecer bien la organización de los contenidos**  
+ Crear directorios chapter ó sección.  Puede incluir un fichero _index.md
+ Crear ficheros de contenido con el comando `hugo new nombre_seccion/nombre_fichero.md`  
+ Los ficheros se crean en la carpeta **content** del directorio raíz del sitio  
+ Las secciones ó capitulos tienen un contenido por defecto especificado en `archetypes/chapter.md`  
+ Los ficheros tienen un contenido por defecto especificado en `archetypes/default.md`  
+ Cada fichero creado tiene al comienzo el **front matter**, encerrado entre dos bloques de 3 líneas - - -  
+ Las **taxonomías** permiten clasificar contenido.  Por defecto, hugo añade las taxonomías **categories** y **tags**

