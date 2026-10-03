---
title: Fil de discussion
keywords:
  - salon
  - textuel
  - fil
  - thread
  - discussion
  - conversation
description: Les fils (threads) ouvrent une "sous-discussion" sur un sujet spécifique, uniquement dans les salons textuels
contributors: [karal, dragrame, cahtounet]
---

Un fil (autrement appelés thread, en anglais) constitue une "sous-discussion".
Ils permettent de parler d'un sujet précis, dans un espace réservé, au sein d'un [salon textuel](/wiki/interface/salons-textuels).

## Création de fils publics et privés

Afin de créer un fil dans un salon textuel, l'utilisateur doit posséder une des permissions :
* "Créer des fils publics", pour pouvoir créer des fils visibles par tous ;
* "Créer des fils privés", afin d'accéder à la création de fils accessibles par invitation uniquement et visibles par les modérateurs ;
* "Gérer les fils", permettant de modérer des fils publics et privés.
Les utilisateurs ayant la permission "Envoyer des messages dans les fils" pourront alors y discuter.

![Création d'un fil](https://i.dfr.gg/hgPX.png)

## Suppression

Pour supprimer un fil, il faut cliquer sur les trois points en haut à droite du fil puis sur "Supprimer le fil".

## Configuration 

Pour configurer un fil, il faut cliquer sur les trois points en haut à droite du fil puis sur "Modifier le fil".
:::note
Il est nécessaire d'avoir créé le fil ou d'avoir la permission "Gérer les fils et les posts" pour pouvoir l'éditer.
:::


### Le nom du fil

Il est possible de modifier le nom d'un fil.

![Modifier le nom](https://i.dfr.gg/G95.png)
:::note
Contrairement aux noms de salons textuels, il est possible de mettre des espaces et des majuscules dans le nom des fils.
:::

### Mode lent

Le mode lent fonctionne de la même manière que celui des salons textuels.
Il permet de bloquer l'envoi consécutif de messages par un utilisateur sous la durée choisie.
Les utilisateurs avec la permission "Ignorer le mode lent" sont exemptés de cette limitation.
Ce paramètre est réservé à la permission "Gérer les fils".

![Mode lent](https://i.dfr.gg/QY3E.png)

### Le temps avant fermeture

Ce paramètre permet de choisir le temps maximum sans activité avant l'archivage automatique du fil.

![Délai avant fermeture](https://i.dfr.gg/vEZg.png)

## L'archivage de fils

Un fil est fermé automatiquement après le temps avant archivage défini ou bien manuellement par un membre qui a la permission "Gérer les fils et les posts" ou par le créateur du fil.
Les fils archivés peuvent être consultés ou rouverts à tout moment.

![Fermeture d'un fil](https://i.dfr.gg/ob8Z.png)
:::note
Un fil peut aussi être verrouillé par un utilisateur disposant de la permission "Gérer les fils et les posts", ce qui empêche toute interaction dans celui-ci pour les membres.
:::

## Les permissions

Voici la liste des permissions liées aux fils :
- Créer des fils publics : permet de créer de nouveaux fils publics.
- Créer des fils privés : permet de créer de nouveaux fils privés.
- Envoyer des messages dans les fils : permet d'envoyer des messages dans tous les types de fils. 
- Gérer les fils et les posts : capacité d'activer le mode lent, de supprimer et de fermer, verrouiller et déverrouiller les fils.

### Autres options

 - NSFW : Un fil est configuré comme NSFW (Not Safe For Work) si son salon parent l'est. Un message apparaît pour demander à l'utilisateur de confirmer qu'il a bien 18 ans car certaines images/liens/contenus dans le fil peuvent choquer un public non averti.
 - Spoiler : Si l'option est activée, un message apparaît pour demander à l'utilisateur s'il souhaite voir le contenu du fil, afin de le prévenir qu'il peut contenir des spoilers.
 - Tout le monde peut inviter : Uniquement disponible pour les fils privés, cette option permet, si désactivée, d'éviter que les utilisateurs autres que le créateur du fil ou des modérateurs puissent ajouter d'autres membres au fil en les mentionnant.
