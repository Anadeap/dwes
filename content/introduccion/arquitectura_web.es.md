---
title: "1.2 Arquitectura web"
date: 2021-11-07T20:21:56+01:00
draft: false
weight: 3
---
> La arquitectura web es la estructura de nuestro producto final.  Es la organización del código. Se va perfilando en todo su desarrollo.  Hay que decidir al principio que herramientas ó tecnologías utilizar.  

> **Capas de una aplicación web:** 
>> **Capa de acceso a datos**: almacena la información de la aplicacion en una base de datos.  
>> **Capa intermedia**: programa la funcionalidad de la aplicación.  
>> **Capa cliente**: engloba todo lo relacionado con la interfaz de usuario, la parte visible.
### Componentes de una aplicación web:
1. **Un servidor web** para recibir las peticiones de los clientes web.
+ Un servidor web es un software encargado de recibir una solicitud por la red.
+ En una red de tipo TCP/IP, la solicitud se recibe usando el protocolo http.
+ Responder a dicha solicitud implica verificar permisos, ejecutar script...
+ Y generar un mensaje de respuesta, página html normalmente, usando el protocolo http.
2. **Un servidor de Bases de datos**
+ El servidor de bases de datos suele estar en un servidor específico para ese cometido.
3. **Un módulo de ejecución de código en el servidor**
+ Genera la página web resultante.
+ Es necesario tener instalado un módulo en el servidor que ejecute el código antes de mandar la respuesta al cliente.
4. **Un cliente**
+ Inicia el proceso.  Suele ser un navegador.
+ Recibe la respuesta del servidor.
+ Interpreta las etiquetas de html y aplica el estilo css
+ Ejecuta el código JavaScript
5. **Lenguajes de programación**
+ Necesarios en el lado cliente y en servidor.
### Tecnologías web
> Son herramientas que se usan para la arquitectura  

Ejemplos:  
![ap_web](/images/tec_web.png) 
{{%attachments title="Arquitectura web" style="blue" /%}}

