---
title: Les rôles
keywords:
  - serveur
  - role
  - rank
  - permissions
description: Paramétrage des rôles de serveur Discord
contributors: [autumn, ichii, dreas, feoxy, volcanofr]
short_slug: roles
---

Sur un serveur Discord, il est possible de créer et personnaliser des rôles ainsi que les attribuer aux membres du serveur.

Pour avoir accès à la liste des rôles, afin de les paramétrer, il faut :
1. se rendre dans les paramètres du serveur ;
2. cliquer sur la section "Rôles".

On peut, à cet endroit, avoir une liste des rôles ainsi que leur permission respective.
On peut aussi y configurer les permissions par défaut du serveur - les permissions du "rôle" `@everyone`.

[//] # (à insérer : un gif montrant les 2 étapes puis l'affichage du menu)

:::caution Attention !
Les permissions des salons sont prioritaires quand elles sont vertes. (voir articles permissions rôles et permissions générales)
:::

## Le rôle `@everyone`

Affiché tout en haut de la liste des rôles à l'arrivée dans le menu, au-dessus même de la recherche des rôles,

![Trouver le rôle everyone](https://cdn.discordapp.com/attachments/1189223435772121149/1193312006002982932/dfr-wiki_role-everyone.png)

ce rôle configure les permissions de base des membres du serveur.

Attribué à **tous** les membres, il est juste invisible.
C'est d'ailleurs pour cette dernière information que l'on peut uniquement configurer les permissions.
Il est aussi impossible de supprimer ou de se retirer ce rôle.

## La couronne du propriétaire

Une couronne est affichée à côté du nom du propriétaire. Une seule condition s'applique à l'apparition de cette couronne :
- si un autre rôle ayant la permission administrateur est affiché séparément, la couronne disparaît.

![Couronne du propriétaire](https://i.discord.fr/75f7.png)
_Avec la couronne_

![Absence de la couronne](https://i.discord.fr/xiTu.png)
_Sans la couronne_

:::note
Les propriétaires de serveur sont considérés comme étant au-dessus de tout les rôles, et ayant la permission "Administrateur".
:::

## Création d'un rôle

Afin de créer un rôle, deux options s'offrent à vous.

1. Cliquer sur le bouton "Création de rôle", à côté de la recherche, dans le menu principal des rôles

![Créer un rôle à partir du menu principal](https://cdn.discordapp.com/attachments/1189223435772121149/1193312006002982932/dfr-wiki_role-everyone.png)

2. À côté du bouton "RETOUR", cliquer sur le "+", dans le menu de configuration des rôles

![créer un rôle à partir du menu de configuration](https://cdn.discordapp.com/attachments/1189223435772121149/1193319835694792774/dfr-wiki_creation-role.png)

Un rôle nouvellement créé s'appellera "nouveau rôle".
Sa couleur est "invisible" et aucune permission ne lui est attribuée par défaut.
Pour personnaliser ce rôle, il faut donc le configurer.

![newrole](https://i.discord.fr/AbWQ.png)

Un rôle peut être modifié/créé à tout moment par un membre, à condition que celui-ci ait :
- la permission "Gérer les rôles" ;
- un rôle plus élevé que le rôle qu'il souhaite modifier.
- les permissions qu'il souhaite lui-même attribuer.

Sans la permission "Gérer le serveur", aucune modification aux rôles ne pourra être appliquée et la section sera cachée.

Si un rôle est plus élevé ou égal au rôle le plus haut du membre, et que le celui-ci n'est pas propriétaire du serveur, un cadenas sera affiché entre la couleur et le nom du rôle. Aucune modification sur le rôle ne pourra être appliquée sur le rôle.

Les permissions que l'on ne possède pas n'ont pas la possibilité d'être cochés, les cases sont grisées.

:::note
- Il est nécessaire d'enregistrer les modifications pour qu'elles soient effectives.
- Les membres ayant la permission "Adminsitrateur" sont considérés comme ayant toutes les permissions.
:::

## Les permissions

Il est possible de configurer les permissions de chaque rôle. Des descriptions aux paramètres sont présents sur Discord.

Une permission attribuée à un rôle s'appliquera à tout membre ayant ce rôle, même si des rôles plus élevés qui ne donnent pas la permission leur sont donnés.

:::caution Attention !
Les permissions des salons sont toujours prioritaires sur les rôles.
:::

> Pour en savoir plus sur les permissions, rendez-vous sur [les pages dédiées aux permissions](/gestion-serveur/permissions).

## Les couleurs

La couleur "invisible" est celle par défaut. Si un rôle placé en dessous d'un rôle invisible a une couleur, c'est celle-ci qui apparaîtra sur le profil d'un utilisateur. Comme ceci :

![Couleur affichée lors de multiples rôles](https://i.discord.fr/cnM8.png)

En plus des 20 couleurs prédéfinies, une roue de sélection de couleurs est disponible afin de permettre une personnalisation complète de la couleur.

![Customisation de la couleur](https://i.discord.fr/BZ8z.png)

Cependant, Discord ne préviendra pas si une couleur sera illisible dans vos salons écrits. Seul un aperçu en thême clair/sombre est visible.

![Ullisibilité d'un pseudonyme coloré](https://i.discord.fr/FaQ4.png)


## Les paramètres du rôle

![Paramètres du rôle](https://i.discord.fr/jvn.png)

### • Afficher les membres ayant ce rôle séparément des autres membres en ligne

![Affichage séparé du rôle](https://i.discord.fr/xiTu.png)

### • Permettre à tout le monde de @mentionner ce rôle
Si activé, chaque utilisateur ou un rôle ayant la permission de mentionner everyone/here et tous les rôles du serveur peut mentionner ce rôle.

![Mentionner un rôle](https://i.discord.fr/iRI.png)

## Icône de rôle

Depuis peu, il est possible d'ajouter des badges de rôle personnalisé. On ne peut en mettre qu'un par rôle et pour cela le niveau 2 de boost est nécessaire [(Voir Article Nitro Boosting)](https://discord.fr/wiki/nitro-jeux/boost-serveur/boost/). /!\ Si L'utilisateur possède plusieurs rôles, seul le badge du rôle le plus élevé sera affiché à droite dans la liste des membres.

Le panneau de gestion se trouve ici 

![Paneau de Gestion](https://i.discord.fr/veaf.png)

Après configuration du bage, voilà ce que cela donne sur le serveur

![Affichage Serveur](https://i.discord.fr/ey8T.png)

