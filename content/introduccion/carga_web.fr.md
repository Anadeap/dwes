---
title: "1.3 Processus de chargement des pages Web"
date: 2021-11-07T20:22:13+01:00
draft: false
weight: 4
---
**1**. L'utilisateur saisit une **URL** dans le client (navigateur).

**2**. Le navigateur recherche l'**IP** :
+ D'abord dans le cache du navigateur
+ Deuxièmement, dans le cache du système d'exploitation
+ Troisièmement, dans le cache du routeur
+ Quatrièmement, dans le cache du FAI

S'il ne peut pas trouver l'adresse IP, le serveur **DNS** du FAI lance une requête pour trouver l'adresse
IP du serveur sur lequel le nom de domaine est hébergé. La demande est envoyée en petit paquets de données contenant des informations sur le contenu de la demande et l'adresse IP.

**3**. Le navigateur initie une **connexion TCP/IP** au serveur à l'aide de messages de synchronisation (SYN) et d'accusé de réception (ACK).

**4**. Le client envoie une **requête HTTP**.

Le protocole HTTPS implique un autre protocole appelé **TLS** qui fournit l'authentification et le cryptage (le navigateur crypte une pré-clé générée à ce moment avec la clé publique du serveur auquel nous voulons nous connecter. Celle-ci est envoyée au serveur, qui décrypte la pré-clé avec sa clé privée. key - Cryptographie asymétrique : un message crypté avec une clé ne peut être crypté qu'avec sa paire correspondante.Le serveur et le navigateur appliquent un certain algorithme à la pré-clé et obtiennent la même clé de cryptage -).

**5**. Si la requête aboutit, le serveur envoie la **réponse**.

5.1 Dans les **sites Web statiques**, le serveur envoie le contenu de la page en HTML.

Sur les **sites Web dynamiques**, les scripts peuvent être exécutés :

5.2 Programmation **côté client**:

Une fois que le navigateur a téléchargé la page, il **détecte le code** dans le code HTML que le serveur envoie **et l'exécute** (dans le navigateur ou en tant que programme séparé en dehors du navigateur). Par exemple, le navigateur exécute JavaScript à l'intérieur du HTML, traite les balises HTML et applique les styles CSS. Parsing : si nécessaire, demander des ressources au serveur.

5.3 Programmation **côté serveur**:

**Le serveur**, généralement en langage PHP, **interprète le script**, insère le HTML généré par le code directement dans la page web puis l'envoie au client.
Il effectue également des requêtes dans la **Base de données**.

**6**. **Le navigateur traite le DOM et construit la page**, en combinant les informations trouvées dans les données du serveur (le fichier HTML d'origine) et dans les ressources.

Si vous avez besoin d'une requête vers la base de données, afin de ne pas charger une autre page, vous pouvez utiliser la technologie AJAX qui permet à JavaScript d'envoyer des requêtes aux scripts PHP. JavaScript reçoit des chaînes de texte en tant que réponse et, en fonction de la réponse, vous pouvez dessiner de nouveaux éléments GUI ou les modifier.

** 7 **. Le moteur de rendu du navigateur est déterminant lors de l'interprétation des lignes de code. C'est pourquoi il existe des différences dans l'affichage d'une page dans différents navigateurs

{{<mermaid align="center">}}
graph LR;
    A[CLIENT 1-2] -->|TCP/IP| B(SERVEUR 3-4)
    B --> C{5}
    C -->|5.1| D[CLIENT 6-7]
    C -->|5.2| E[CLIENT 6-7]
    C -->|5.3| F[CLIENT 6-7]
{{< /mermaid >}}

