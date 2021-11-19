---
title: "Shortcodes"
date: 2021-11-07T20:45:32+01:00
draft: false
weight: 12
---
### EJEMPLOS DE SHORTCODES
> Un **shortcode** es un fragmento de código html que será renderizado dentro de un fichero md cuando el sistema cargue o renderice la página de contenido
1. **Botones**  
_Botón que enlaza con la web de hugo_   
{{% button href="https://gohugo.io/" icon="fas fa-download" %}}Web de hugo{{% /button %}}

***
2. **Attachments - páginas de descarga**   
| Página | Ubicación attachments |
| ------ | ---------------------- |
|   md   | en directorio con el mismo nombre de la página y acabado en .files |
| directorio | en un directorio files anidado |   

{{%attachments title="Attachments" style="orange" /%}} 
***
3. **Acortar un texto con leer más...**   
Clicar en el texto para expandir
{{%expand "Hugo es uno de los generadores de sitios estáticos de código abierto más populares." %}}Con su increíble velocidad y flexibilidad, Hugo vuelve a hacer divertido la creación de sitios web.{{% /expand%}}
***
4. **Textos remarcados**  
Noticia
{{% notice note %}}
Noticia
{{% /notice %}}
Información
{{% notice tip %}}
Información
{{% /notice %}}
Aviso
{{% notice warning %}}
Aviso
{{% /notice %}}
***
5. **Tabs de diferentes elementos**  
Muy útil para proporcionar fragmentos de código para varios idiomas o proporcionar configuración en diferentes formatos  
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
6. **Enlace a un video de youtube**  
{{< youtube 6H0jLIKe0uw >}}

