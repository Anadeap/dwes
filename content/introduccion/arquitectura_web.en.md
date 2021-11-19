---
title: "1.2 Web architecture and technology"
date: 2021-11-07T20:21:56+01:00
draft: false
weight: 3
---
> The web architecture is the structure of our final product. It is the organization of the code. It is emerging throughout its development. You have to decide at the beginning which tools or technologies to use.

> **Layers of a web application:**
>> **Data access layer**: stores the application information in a database.  
>> **Middle layer**: programs the application's functionality.  
>> **Client layer**: includes everything related to the user interface, the visible part.
### Components of a web application:
1. **A web server** to receive requests from web clients.
+ A web server is a software in charge of receiving a request over the network.
+ In a TCP / IP type network, the request is received using the http protocol.
+ Responding to this request implies checking permissions, executing script ...
+ And generate a response message, normally html page, using the http protocol.
2. **A database server**
+ The database server is usually on a specific server for that purpose.
3. **A code execution module on the server**
+ Generates the resulting web page.
+ It is necessary to have a module installed on the server that executes the code before sending the response to the client.
4. **A client**
+ Starts the process. It is usually a browser.
+ Receive the response from the server.
+ Interpret html tags and apply css style
+ Run the JavaScript code
5. **Programming languages**
+ Necessary on the client and server side.
### Web technologies
> They are tools used for architecture

Examples:
![ap_web](/images/tec_web.png)

