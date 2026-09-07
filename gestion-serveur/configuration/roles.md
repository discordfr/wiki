---
title: Rôles
keywords:
  - rôle
  - permission
  - serveur
  - configuration
description: Les rôles, le point d'entrée à la configuration des permissions et à la customisation des serveurs Discord
contributors: [autumn, ichii, dreas, feoxy, wolfyzdbois, volcanofr]
short_slug: roles
---

Sur un serveur Discord, il est possible de créer et personnaliser des rôles ainsi que les attribuer aux utilisateurs présents.
On peut leur allouer des permissions de base.
Sur un serveur Discord, il est possible de créer et personnaliser des rôles ainsi que les attribuer aux utilisateurs présents.
Les rôles permettent de configurer les [permissions](/wiki/gestion-serveur/permissions) du serveur et celles par défaut des salons.

Pour que les changements soient pris en compte, l'utilisateur configurant le serveur doit sauvegarder ses modifications.

:::warning
Les permissions par défaut liées aux salons sont prioritaires quand elles sont vertes.
:::

Le panneau de gestion des rôles est présent dans les [paramètres du serveur](/wiki/gestion-serveur/configuration), menu disponible en cliquant sur le nom du serveur.

![Accès aux paramètres du serveur](https://i.dfr.gg/89gp.png)

Le menu se présente comme tel :

![Panneau de gestion des rôles](https://i.dfr.gg/CFJY.png)

## Rôle @everyone

![Nom du rôle "@everyone" inchangeable](https://i.dfr.gg/HVd.png)

Ce rôle configure les permissions de base de tous les membres du serveur.
Une permission désactivée sur un rôle en particulier, mais activée sur le rôle everyone, permettra tout de même l'exécution de cette dernière.

:::note
Il n'est pas possible de configurer le nom, l'icône et la couleur de celui-ci, tout comme il est impossible de supprimer ou encore de retirer ce rôle à un membre.
:::

## Création d'un rôle

Il existe deux possibilités pour créer un rôle : via le « + » ou le bouton bleu « Création de rôle ».
Après cela, l'utilsateur créant le rôle est redirigé vers l'interface de personalisation du rôle.

![Créer un rôle via le "+"](https://i.dfr.gg/Oc7f.png) 

![Créer un rôle via le bouton](https://i.dfr.gg/QqbC.png)

Un rôle nouvellement créé s'appelle par défaut « nouveau rôle ».
Sa couleur est "invisible" (transparente) et aucune permission n'est attribuée par défaut.

![Nouveau rôle](https://i.dfr.gg/AbWQ.png)

Un rôle peut être modifié à tout moment par un utilisateur, à condition que celui-ci ait la permission "gérer les rôles" et que son rôle le plus haut se situe au-dessus de celui souhaité.
Si la personne qui effectue les modifications sur un rôle ne dispose pas elle-même de la permission qu'elle souhaite modifier, la case sera grisée et il sera impossible d'interagir avec.

## Les couleurs

La couleur "invisible" est celle par défaut.
Tout rôle ayant comme couleur l'hexadécimal `#99aab5` est considéré "invisible".
Si un rôle placé en dessous d'un rôle invisible a une couleur, c'est celle-ci qui apparaîtra sur le profil d'un utilisateur.

![Transparence avec un rôle de couleur "invisible"](https://i.dfr.gg/cnM8.png)

En plus des 20 couleurs prédéfinies, une roue de couleurs (color wheel) est disponible pour permettre une personnalisation complète de la couleur.

![Sélection personnalisée de couleur](https://i.dfr.gg/BZ8z.png)

Discord ne préviendra pas si une couleur sera illisible dans vos salons écrits.
Cependant, il est possible de vérifier visuellement la correspondance sur thême clair et sombre.

![Illisibilité de couleur au thême sombre](https://i.dfr.gg/FaQ4.png)

Il est également possible de sélectionner un dégradé de couleur parmi 12 dégradés proposés par défaut, ou en sélectionnant deux couleurs dans la roue des couleurs.
La couleur Holographique est également disponible, qui donnera un effet arc-en-ciel pastel.

:::note
La sélection d'un dégradé de couleur ou de la couleur Holographique nécessite d'activer l'avantage "Style de rôles améliorés" pour 3 boosts de serveur dans l'onglet correspondant.
:::

## Les paramètres du rôle

![Paramètres du rôle](https://i.dfr.gg/jvn.png)

### Afficher les membres ayant ce rôle séparément des autres membres en ligne

![Affichage séparé du rôle](https://i.dfr.gg/xiTu.png)

### Permettre à tout le monde de @mentionner ce rôle

Si cette option est activée, tout les utilisateurs du serveur pourront mentionner ce rôle.

![Mentionner un rôle](https://i.dfr.gg/iRI.png)

## Badge de rôle personnalisé 

:::note
Cette fonctionnalité est disponible à partir du niveau 2 de [boost de serveur](/wiki/contenu-payant/boost-serveur).
:::

Le badge du plus haut rôle du membre parmis ceux ayant un badge personnalisé s'affiche de son nom d'affichage dans les discussions.
Sur l'affichage séparé dans la liste des membres, le badge est affiché à gauche du nom du rôle.
Tous les badges de rôles sont visibles à gauche des noms de rôles correspondants dans le profil des membres.

Le panneau de gestion se trouve sous la sélection de couleur :

![Panneau de gestion](https://i.dfr.gg/veaf.png)

Voici le rendu d'un badge de rôle :

![Différents affichages du badge de rôle](https://i.dfr.gg/ey8T.png)

## Les rôles liés

Un rôle lié est un rôle qu'un membre peut obtenir s'il respecte certains prérequis de connexion entre des comptes externes et son compte Discord.

![Configuration du rôle lié](https://i.dfr.gg/v4i6.png)

Le membre pourra ensuite aller dans l'onglet "Rôle lié" dans le menu du serveur, et sélectionner ses rôles, selon les prérequis qu'il respecte.

![Sélection par le membre du rôle lié](https://i.dfr.gg/yicb.png)

:::tip
Il est également possible de créer sa propre connexion avec ses propres prérequis pour son serveur.
La [documentation officielle de Discord Developper Portal](https://discord.com/developers/docs/tutorials/configuring-app-metadata-for-linked-roles) explique comment faire aux développeurs.
:::

## Couronne du propriétaire

Une couronne est affichée à côté du nom du propriétaire.
Si un rôle ayant la permission administrateur affiche séparément le propriétaire, sa couronne disparaît.

- Avec la couronne
  
  ![Couronne du propriétaire](https://i.dfr.gg/75f7.png)

- Sans la couronne
  
  ![Couronne du propriétaire absente](https://i.dfr.gg/xiTu.png)
