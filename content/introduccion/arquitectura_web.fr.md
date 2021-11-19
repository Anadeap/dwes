---
title: "1.2 Architecture et technologie Web"
date: 2021-11-07T20:21:56+01:00
draft: false
weight: 3
---
> L'architecture web est la structure de notre produit final. C'est l'organisation du code. Il émerge tout au long de son développement. Vous devez décider au début quels outils ou technologies utiliser.

> **Couches d'une application web:**
>> **Couche d'accès aux données**: stocke les informations de l'application dans une base de données.  
>> **Couche intermédiaire**: programme les fonctionnalités de l'application.  
>> **Couche client**: comprend tout ce qui concerne l'interface utilisateur, la partie visible.
### Composants d'une application Web:
1. **Un serveur Web** pour recevoir les requêtes des clients Web.
+ Un serveur web est un logiciel chargé de recevoir une requête sur le réseau.
+ Dans un réseau de type TCP/IP, la requête est reçue via le protocole http.
+ Répondre à cette requête implique de vérifier les autorisations, d'exécuter le script...
+ Et générer un message de réponse, normalement une page html, en utilisant le protocole http.
2. **Un serveur de base de données**
+ Le serveur de base de données se trouve généralement sur un serveur spécifique à cet effet.
3. **Un module d'exécution de code sur le serveur**
+ Génère la page Web résultante.
+ Il est nécessaire d'avoir un module installé sur le serveur qui exécute le code avant d'envoyer la réponse au client.
4. **Un client**
+ Démarre le processus. Il s'agit généralement d'un navigateur.
+ Recevez la réponse du serveur.
+ Interpréter les balises html et appliquer le style CSS
+ Exécutez le code JavaScript
5. **Langages de programmation**
+ Nécessaire côté client et côté serveur.
### Technologies Web
> Ce sont des outils utilisés pour l'architecture

Exemples:
![ap_web](/images/tec_web.png)

