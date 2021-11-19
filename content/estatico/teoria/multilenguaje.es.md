---
title: "Multilenguaje"
date: 2021-11-07T20:50:09+01:00
draft: false
weight: 14
---
**Establecer diferentes idiomas en hugo**  
**1. Modificar config.toml**  
![captura_idiomas](/images/captura_idiomas.png)
***
**2. Se puede establecer un idioma por defecto**
![captura_pordefecto](/images/captura_pordefecto.png)
***
**3. Cambiando la página por defecto**
+ Hay que establecer el contenido de la página por defecto en los idiomas
+ En **learn**, si no hay contenido en "content", este contenido está en el fichero **index.html**, ubicado en `themes/learn/layouts`
+ Esta plantilla está preparada para inglés y francés, por lo que hay que añadir una estructura de control para incluir otro idioma
***
**4. Cambiando valores a través de variables**
+ Se pueden especificar palabras para ser traducidas
+ En **i18n**, las 2 primeras letras de los ficheros identifican el idioma
+ Estos ficheros traducen y el sistema obtiene el valor del fichero, usando la función de traducción de hugo
![captura_traduccion](/images/captura_traduccion.png)
***
**5. Menús en varios idiomas**
+ Establecer en config.toml: 
```
   [Languages]
   [Languages.es]
   ...
   [[Languages.es.menu.shortcuts]]
   ```
***
**6. Añadiendo páginas traducidas**
> Una forma de especificar las traducciones es nombrar cada fichero correspondiente a una página  referenciando a los idiomas  
```
fichero.es.md
fichero.en.md
fichero.fr.md
```  

+ En config.toml, indicar, con la variable **contentDir**, el directorio dónde se ubican los ficheros traducidos al idioma:
```
   [Languages]
   [Languages.es]
   ...
      ContentDir = "content"
```

