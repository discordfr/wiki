---
title: Applications autorisées
keywords:
  - application
  - app
  - bot
  - autorisé
  - autorise
  - sécurité
  - securite
description: Les applications autorisées sur son compte Discord, via OAuth2.
contributors: [moonrise, ben, dragrame]
short_slug: OAuth2
---

Les applications sont créées sur le [portail développeurs](https://discord.com/developers/applications) de Discord.
Elles permettent d'intéragir avec Discord avec un programme informatique.

## Autoriser une application

Pour autoriser une application à accéder à son compte, il faut se rendre sur un lien similaire à « `https://discord.com/oauth2/authorize` ».
Chaque application a un lien différent en fonction de son **identifiant**, renseigné dans l'URL.

![Autoriser une application](https://i.dfr.gg/twpp.png)

### Permissions

Les applications peuvent demander l'accès à plusieurs permissions, voici les plus communes :

* Ajouter un bot sur un serveur
* Créer des slash commands sur un serveur
* Lire les informations de l'utilisateur connecté telles que : identifiant, nom d'utilisateur, discriminateur (#0000), avatar, bannière (couleur et image), authentification à deux facteurs, souscription à [Nitro](/wiki/contenu-payant/abonnements-nitro), badges.
* Lire l'adresse email de l'utilisateur connecté
* Lire les [connexions officielles](/wiki/compte-utilisateur/connexions-externes/passeport) de l'utilisateur connecté
* Lire la liste des serveurs de l'utilisateur connecté
* Rejoindre des serveurs pour l'utilisateur connecté

:::note
Une application ne pourra jamais lire ou envoyer de messages à la place de l'utilisateur.
:::

## Révoquer une application

Les applications sont faites pour rendre l'expérience sur Discord meilleure, mais elles peuvent toutefois se révéler oppressantes ou inutiles…
Dans ce cas, il est possible de **révoquer une application** dans les **paramètres du compte**, section « `Applications autorisées` ».
Il faut alors **survoler l'application** concernée avec la souris et cliquer sur le bouton rouge « `Retirer l'autorisation` » qui apparaît.

![Révoquer une application](https://i.dfr.gg/soip.png)

---

:::info L'article nécessite des modifications
* Compléter l'article : lister tous les [champs d'OAuth2](https://docs.discord.com/developers/topics/oauth2#shared-resources-oauth2-scopes).

Ce projet communautaire vise à offrir un contenu librement réutilisable, que chacun peut modifier et améliorer.
Pour contribuer, munissez-vous d'un compte GitHub et rendez-vous sur notre [page de contribution](/wiki/contribuer).
:::
