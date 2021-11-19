---
title: "1.3 Proceso de carga de una página web"
date: 2021-11-07T20:22:13+01:00
draft: false
weight: 4
---
**1**.	El usuario introduce una **URL** en el cliente (navegador).   

**2**.	El navegador busca la **IP**:
+ Primero en el caché del navegador
+ Segundo, en el caché del sistema operativo
+ Tercero, en el caché del router
+ Cuarto, en el caché de ISP  

Si no encuentra la IP, el servidor **DNS** del ISP inicia una consulta para encontrar la dirección IP del servidor donde se aloja el nombre del dominio. La solicitud se envía en pequeños 
paquetes de datos que contienen información sobre el contenido de la solicitud y la dirección 
IP.  

**3**.	El navegador inicia una **conexión TCP/IP** con el servidor mediante mensajes de sincronización (SYN) y reconocimiento (ACK).  

**4**.	El cliente envía una **solicitud HTTP**.  

El protocolo HTTPS involucra otro protocolo llamado **TLS** que proporciona autenticación y encriptación (el navegador cifra una preclave generada en el momento con la clave pública del servidor al que nos queremos conectar). Eso se envía al servidor, que descifra la preclave con su clave privada - criptografía asimétrica: un mensaje cifrado con una clave sólo puede ser cifrado con su par correspondiente. El servidor y el navegador aplican un cierto algoritmo a la preclave y obtienen la misma clave de cifrado - ).

**5**.	Si la solicitud tiene éxito, el servidor envía la **respuesta**.  

5.1 En las **webs estáticas**, el servidor envía el contenido de la página en HTML.  

En las **webs dinámicas**, los scripts se pueden ejecutar:

5.2 Programación **del lado del cliente**:

Después de que el navegador descarga la página, **detecta el código** dentro del HTML que el servidor envía **y lo ejecuta** (dentro del navegador o como programa separado fuera del navegador).  Por ejemplo, el navegador ejecuta JavaScript que está dentro del HTML, procesa las etiquetas del HTML y aplica estilos CSS.  Parsing: si es necesario, solicita recursos al servidor.

5.3 Programación **del lado del servidor**:

**El servidor**, normalmente en lenguaje PHP, **interpreta el script**, inserta el HTML generado por el código directamente en la página web y luego lo envía al cliente.
También hace consultas a la **Bases de Datos**.

**6**.	**El navegador procesa el DOM y construye la página**, combinando la información encontrada en los datos del servidor (el archivo HTML original) y en los recursos.

Si se necesita una consulta a la Base de Datos, para no cargar otra página, se puede utilizar la tecnología AJAX que permite a JavaScript mandar peticiones a scripts de PHP. JavaScript recibe como respuesta cadenas de texto, y en base a la respuesta puede dibujar nuevos elementos de la interfaz gráfica o cambiarlos. 

**7**.	El motor de renderizado del navegador es determinante al interpretar las líneas de código.  Es por eso que hay diferencias en la visualización de una página en distintos navegadores

{{<mermaid align="center">}}
graph LR;
    A[CLIENTE 1-2] -->|TCP/IP| B(SERVIDOR 3-4)
    B --> C{5}
    C -->|5.1| D[CLIENTE 6-7]
    C -->|5.2| E[CLIENTE 6-7]
    C -->|5.3| F[CLIENTE 6-7]
{{< /mermaid >}}

