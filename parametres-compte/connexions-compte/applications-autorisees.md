---
id: applications-autorisees
title: Les applications autorisées
keywords:
  - discord
  - sécurité
  - applications
  - autorisées
  - tutoriel
description: Les applications autorisées sur son compte discord
---
# Les applications autorisées

Les applications sont créées sur le [portail développeurs](https://discord.com/developers/) de Discord. Elles permettent de "se connecter avec discord", comme le font plusieurs tableaux de bord de bots Discord.

## Autoriser une application
Pour autoriser une application à accéder à son compte, il faut se rendre sur un lien similaire à `https://discord.com/oauth2/authorize`. Chaque application a un lien différent en fonction de son **identifiant**, renseigné dans l'url.

![Autoriser une application](https://i.discord.fr/twpp.png)


### Permissions
Les applications peuvent demander l'accès à plusieurs permissions, voici les plus communes :
- Ajouter un bot sur un serveur
- Créer des slash commands sur un serveur
- Lire les informations de l'utilisateur connecté telles que : identifiant, nom d'utilisateur, discriminateur (#0000), avatar, bannière (couleur et image), authentification à deux facteurs, souscription à [Nitro](https://discord.fr/wiki/nitro-jeux/nitro/abonnements/), badges.
- Lire l'adresse email de l'utilisateur connecté
- Lire les [connexions officielles](https://discord.fr/wiki/parametres-compte/connexions-compte/connexion-officielle/) de l'utilisateur connecté
- Lire la liste des serveurs de l'utilisateur connecté
- Rejoindre des serveurs pour l'utilisateur connecté

:::note Une application ne pourra jamais lire ou envoyer de messages à votre place. :::

## Révoquer une application
Les applications sont faites pour rendre l'expérience sur Discord meilleure, mais elles peuvent toutefois oppressantes ou inutiles... Dans ce cas, il est possible de révoquer une application dans les paramètres de compte, section `Applications autorisées`. Il faut alors survoler l'application concernée avec la souris et cliquer sur le bouton rouge `Retirer l'autorisation` qui apparaît.

![Révoquer une application](https://i.discord.fr/soip.png)
