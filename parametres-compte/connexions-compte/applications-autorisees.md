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

Les applications sont créées sur le [portail développeurs](https://discord.dev) de Discord. Elles permettent de "se connecter avec discord", comme le font plusieurs dashboards de robots Discord.

# Autoriser une application
Pour autoriser une application à accéder à son compte, il faut se rendre sur un lien similaire à `https://discord.com/oauth2/authorize?scope=identify&client_id=563836644579606528&response_type=code&redirect_uri=https%3A%2F%2Fsupport.discord.fr%2Fcallback`. Chaque application a un lien différent en fonction de son **identifiant**, renseigné dans le champ `client_id=` de l'url.

![Autoriser une application](https://i.discord.fr/13rP.png)


## Permissions
Les applications peuvent nécessiter plusieurs permissions, en voici la liste des plus communes :
- Ajouter un robot sur un serveur
- Créer des slash commands sur votre serveur
- Lire vos informations telles que : identifiant, nom d'utilisateur, discriminateur (#0000), avatar, bannière (couleur et image), authentification à deux facteurs, souscription à [Nitro](https://discord.fr/wiki/nitro-jeux/nitro/abonnements/), badges.
- Lire votre adresse email
- Lire vos [connexions officielles](https://discord.fr/wiki/parametres-compte/connexions-compte/connexion-officielle/)
- Lire la liste de vos serveurs
- Rejoindre des serveurs pour vous

:::note Une applications ne pourra jamais lire ou envoyer des messages à votre place. :::

# Révoquer une application
Les applications sont faites pour rendre l'expérience sur Discord meilleure, mais elles peuvent toutefois être trop bien... Dans ce cas, il est possible de révoquer une application dans les paramètres de compte, section `Applications autorisées`. Il faut alors survoler l'application concernée avec la souris et cliquer sur le bouton rouge `Retirer l'autorisation` qui apparaît.

![Révoquer une application](https://i.discord.fr/soip.png)
