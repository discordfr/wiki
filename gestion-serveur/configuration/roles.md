---
title: Les rôles
keywords:
  - discord
  - serveur
  - tutoriel
  - roles
  - permissions
description: Les rôles sur un serveur Discord
contributors: [autumn, ichii, dreas, feoxy, wolfyzdbois]
short_slug: Roles
---

Sur un serveur Discord, il est possible de créer et personnaliser des rôles ainsi que les attribuer aux utilisateurs présents.
On peut leur allouer des permissions de base.
Il est nécessaire d'enregistrer les modifications pour qu'elles soient effectives.

:::caution Attention !
Les permissions des salons sont prioritaires quand elles sont vertes. (voir articles permissions rôles et permissions générales)
:::

Le panneau de gestion des rôles est présent dans le menu des paramètres, disponible dans le menu qui s'affiche en cliquant sur le nom du serveur.

![où est le panneau de gestion des rôles](https://i.dfr.gg/89gp.png)

Il se présente ainsi.

![Panneau de gestion des rôles](https://i.dfr.gg/CFJY.png)


## Petit point sur le rôle @everyone

![rôle everyone](https://i.dfr.gg/HVd.png)

Ce rôle configure les permissions de base des membres du serveur et est attribué par défaut. Les membres sans aucun rôle seront directement affectés par les permissions de ce dernier. Une permission désactivée sur un rôle en particulier, mais activée sur le rôle everyone, permettra tout de même l'exécution de cette dernière.

:::note Note
Il n'est pas possible de configurer le nom, l'icône et la couleur de celui-ci, tout comme il est impossible de supprimer ou encore de se retirer ce rôle.
::: 


## Création d'un rôle

Il existe deux possibilités pour créer un rôle : via le « + » ou via le bouton bleu « Création de rôle ». Après cela, vous serez redirigé vers la page des rôles pour la configuration.

![créer un rôle](https://i.dfr.gg/Oc7f.png) 

![créer un rôle autrement](https://i.dfr.gg/QqbC.png)

Un rôle nouvellement créé s'appelle par défaut « nouveau rôle ». Sa couleur est "invisible" et les mêmes permissions que le rôle everyone lui sont attribuées par défaut. 

:::tips
Pour gagner du temps et ne pas oublier des petits détails qui qui peuvent à l'avenir déranger le bon fonctionnement du serveur, il est important de bien configurer les permissions du rôle everyone avant de créer d'autres rôles, vous gagnerez du temps et vous n'oublierez pas les petits détails
:::
vtre
![newrole](https://wolfyzdfile.fr/20260127_004224_image_4c213949.png)

Un rôle peut être modifié à tout moment par un utilisateur, à condition que celui-ci ait la permission "gérer les rôles" et qu'il dispose des permissions qu'il souhaite lui-même attribuer. Si la personne qui effectue les modifications sur un rôle ne dispose pas lui-même de la permission qu'il souhaite attribuer, la case sera grisée et il sera impossible d'interagir avec. Par exemple si l'auteur de l'édition ne dispose pas de la permission "mentionner everyone", il ne pourra donc pas l'attribuer à un autre rôle.


## Les couleurs
La couleur "invisible" est celle par défaut. Si un rôle placé en dessous d'un rôle invisible a une couleur, c'est celle-ci qui apparaîtra sur le profil d'un utilisateur.

![rôle invisible et rôle visible](https://i.dfr.gg/cnM8.png)

En plus des 20 couleurs prédéfinies, une roue de couleurs (color wheel) est disponible pour permettre une personnalisation complète de la couleur.

![color wheel](https://i.dfr.gg/BZ8z.png)

Cependant, Discord ne préviendra pas si une couleur sera illisible dans vos salons écrits. Une astuce est de vérifier que le rôle sera bien lisible, aussi bien sur thème clair que sombre.

![illisibilité de couleur](https://i.dfr.gg/FaQ4.png)

Il est également possible de sélectionner un dégradé de couleur parmi 12 dégradés proposés par défaut, ou en sélectionnant deux couleurs dans la roue des couleurs. La couleur Holographique est également disponible, qui donnera un effet arc-en-ciel.

:::note Avantage Boost
La sélection d'un dégradé de couleur ou de la couleur Holographique nécessite d'activer l'avantage "Style de rôles améliorés" pour 3 boosts de serveur dans l'onglet correspondant.
:::

## Les paramètres du rôle

![Paramètres du rôle](https://i.dfr.gg/jvn.png)

### • Afficher les membres ayant ce rôle séparément des autres membres en ligne

![Affichage séparé du rôle](https://i.dfr.gg/xiTu.png)

### • Permettre à tout le monde de @mentionner ce rôle

Si cette option est activée, tout les utilisateurs du serveur pourront mentionner ce rôle.

![Mentionner un rôle](https://i.dfr.gg/iRI.png)

## Badge de rôle personnalisé 

Depuis peu, il est possible d'ajouter des badges de rôle personnalisé. On ne peut en mettre qu'un par rôle et pour cela le niveau 2 de boost est nécessaire [(Voir Article Nitro Boosting)](/wiki/contenu-payant/boost-serveur). /!\ Si L'utilisateur possède plusieurs rôles, seul le badge du rôle le plus élevé sera affiché à droite dans la liste des membres.

Le panneau de gestion se trouve ici 

![Panneau de Gestion](https://i.dfr.gg/veaf.png)

Après configuration du badge, voilà ce que cela donne sur le serveur

![Affichage Serveur](https://i.dfr.gg/ey8T.png)

## Les rôles liés

Un rôle lié est un rôle qu'un membre peut obtenir s'il respecte certains prérequis de connexion entre des comptes externes et son compte Discord.

![Configuration du rôle lié](https://wolfyzdfile.fr/20260127_003735_image_3b3692ac.png)

Le membre pourra ensuite aller dans l'onglet "Rôle lié" dans le menu du serveur, et sélectionner ses rôles, selon les prérequis qu'il respecte.

![Sélection par le membre du rôle lié](https://wolfyzdfile.fr/20260127_003856_image_2df1cadf.png)

:::tip
Il est également possible de créer sa propre connexion avec ses propres prérequis pour son serveur. [La documentation officielle de Discord Developper Portal](https://discord.com/developers/docs/tutorials/configuring-app-metadata-for-linked-roles) explique comment faire. 

## Petit point sur la couronne

Une couronne est affichée à côté du nom du propriétaire.
Si un autre rôle ayant la permission administrateur est affiché séparément, la couronne disparaît.

• Avec la couronne

![Couronne du propriétaire](https://i.dfr.gg/75f7.png)

• Sans la couronne

![Couronne du propriétaire absente](https://i.dfr.gg/xiTu.png)