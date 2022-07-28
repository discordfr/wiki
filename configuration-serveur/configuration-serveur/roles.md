---
id: roles
title: Les rôles
keywords:
  - discord
  - serveur
  - tutoriel
  - roles
  - permissions
description: Les rôles sur un serveur Discord
---

Sur un serveur Discord, il est possible de créer et personnaliser des rôles ainsi que les attribuer aux utilisateurs présents.
On peut leur allouer des permissions de base.
Il est nécessaire d'enregistrer les modifications pour qu'elles soient effectives.

:::caution Attention !
Les permissions des salons sont prioritaires quand elles sont vertes. (voir article des [permissions générales](https://discord.fr/wiki/configuration-serveur/permissions/generales/))
:::

Le panneau de gestion des rôles est trouvable à cet endroit.

![où est le panneau de gestion des rôles](https://i.discord.fr/89gp.png)

Il se présente ainsi.

![Panneau de gestion des rôles](https://i.discord.fr/CFJY.png)


## Petit point sur le rôle @everyone

![rôle everyone](https://i.discord.fr/HVd.png)

Ce rôle configure les permissions de base des membres du serveur et est attribué par défaut. Les membres sans aucun rôle seront directement affectés par les permissions de ce dernier. Une permission désactivée sur un rôle en particulier, mais activée sur le rôle everyone, permettra tout de même l'exécution de cette dernière.

:::note Note
Il n'est pas possible de configurer le nom, l'icône et la couleur de celui-ci, tout comme il est impossible de supprimer ou encore de se retirer ce rôle - il est invisible mais bien présent chez tout le monde.
::: 


## Petit point sur la couronne

Une couronne est affichée à côté du nom du propriétaire.
Si un autre rôle ayant la permission administrateur est affiché séparément, la couronne disparaît.

• Avec la couronne

![Couronne du propriétaire](https://i.discord.fr/75f7.png)

• Sans la couronne 

![Couronne du propriétaire absente](https://i.discord.fr/xiTu.png)

## Création d'un rôle
Pour créer un rôle, vous avez maintenant deux possibilités de le faire ! Il faut soit cliquer sur le petit plus à côté de « retour », juste ici :

![créer un rôle](https://i.discord.fr/Oc7f.png) 

Soit vous avez la possibilité de cliquer sur le bouton bleu « Création de rôle ». Après cela vous serez redirigé vers la page des rôles pour la configuration.

![créer un rôle autrement](https://i.discord.fr/QqbC.png)

Un rôle nouvellement créé s'appelle par défaut « nouveau rôle ». Sa couleur est "invisible" et les mêmes permissions que le rôle everyone lui sont attribuées par défaut. Pensez donc à bien configurer votre rôle everyone avant de créer le reste de vos rôles, vous gagnerez du temps et vous n'oublierez pas les petits détails qui peuvent à l'avenir déranger le bon fonctionnement de votre serveur.

![newrole](https://i.discord.fr/AbWQ.png)

Un rôle peut être modifié à tout moment par un utilisateur, à condition que celui-ci ait la permission "gérer les rôles" et qu'il dispose des permissions qu'il souhaite lui-même attribuer. Si la personne qui effectue les modifications sur un rôle ne dispose pas lui-même de la permission qu'il souhaite attribuer, la case sera grisée et il sera impossible d'interagir avec. Par exemple si l'auteur de l'édition ne dispose pas de la permission "mentionner everyone", il ne pourra donc pas l'attribuer à un autre rôle.


## Les couleurs
La couleur "invisible" est celle par défaut. Si un rôle placé en dessous d'un rôle invisible a une couleur, c'est celle-ci qui apparaîtra sur le profil d'un utilisateur. Comme ceci :

![rôle invisible et rôle visible](https://i.discord.fr/cnM8.png)

En plus des 20 couleurs prédéfinies, une roue de couleurs (color wheel) est disponible pour permettre une personnalisation complète de la couleur. Il est aussi possible d'insérer une [couleur hexadécimale](https://45secondes.fr/code-hexadecimal-pour-les-couleurs-tout-sur-la-definition-des-couleurs-hexadecimales/).

![color wheel](https://i.discord.fr/BZ8z.png)

Cependant, Discord ne préviendra pas si une couleur sera illisible dans vos salons écrits. Une simple prévisualisation dans la modification du rôle est possible (thême clair/foncé).

## Les paramètres du rôle

![Paramètres du rôle](https://i.discord.fr/jvn.png)

### • Afficher les membres ayant ce rôle séparément des autres membres en ligne

![Affichage séparé du rôle](https://i.discord.fr/xiTu.png)

### • Permettre à tout le monde de @mentionner ce rôle
Si activé, chaque utilisateur ou un rôle ayant la permission de mentionner everyone/here et tous les rôles du serveur peut mentionner ce rôle.

![Mentionner un rôle](https://i.discord.fr/iRI.png)

## Badge de rôle personnalisé 

Il est aussi possible d'ajouter des badges de rôle personnalisé. On ne peut en mettre qu'un par rôle, et pour débloquer cette fonctionaté : le serveur doit être au niveau 2 de boost [(Voir Article Nitro Boosting)](https://discord.fr/wiki/nitro-jeux/boost-serveur/boost/).
:::caution À noté
Si L'utilisateur possède plusieurs rôles ayant des badges, seul le badge le plus élevé dans la liste des rôles sera affiché dans les discussions textuelles.
:::


Après configuration du bage, voilà ce que cela donne sur le serveur

![Affichage Serveur](https://i.discord.fr/ey8T.png)

