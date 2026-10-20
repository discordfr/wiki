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

L'utilisateur disposant de la permission "Gérer les fils" peut supprimer un fil de plusieurs façons :

* Cliquer sur les trois points en haut à droite du fil, puis sélectionner "Supprimer le fil" ;
* Faire un clic droit sur le nom du fil dans la liste des salons, puis cliquer sur "Supprimer le fil" ;
* Cliquer sur la bobine de fil en haut à droite du salon parent, faire un clic droit sur le nom du fil, puis sélectionner "Supprimer le fil" ;
* Cliquer sur le nom du serveur, sélectionner "Fils actifs", faire un clic droit sur le nom du fil, puis sélectionner "Supprimer le fil".

![Suppression d'un fil](https://i.dfr.gg/qnTv.png)

## Configuration et personnalisation

L'utilisateur possédant la permission "Gérer les fils" ou le créateur du fil peuvent accéder au menu de configuration de plusieurs façons :

* Cliquer sur les trois points en haut à droite du fil, puis sélectionner "Modifier le fil" ;
* Faire un clic droit sur le nom du fil dans la liste des salons, puis cliquer sur "Modifier le fil" ;
* Cliquer sur la bobine de fil en haut à droite du salon parent, faire un clic droit sur le nom du fil, puis sélectionner "Modifier le fil" ;
* Cliquer sur le nom du serveur, sélectionner "Fils actifs", faire un clic droit sur le nom du fil, puis sélectionner "Modifier le fil".

### Nom du fil

Il est possible de modifier le nom du fil sélectionné.

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

### Fermeture

Un fil est **fermé automatiquement après une durée** configurée sans nouveau ni modification de message, ni modification réaction aux messages.

La durée peut être configurée par l'utilisateur ayant créé le fil, ou les utilisateurs ayant la permission "Gérer les fils".

Une durée par défaut est définie dans les paramètres du salon textuel.

![Délai avant fermeture](https://i.dfr.gg/vEZg.png)

Un fil peut aussi être **fermé manuellement** par les mêmes utilisateurs.

![Fermeture d'un fil](https://i.dfr.gg/ob8Z.png)

:::note
Un fil fermé peut être rouvert par tous les utilisateurs ayant accès à ce dernier, y compris les utilisateurs ne l'ayant pas rejoint.
Il est aussi rouvert automatiquement si une activité est détectée.
:::

### Verrouillage

Un fil peut être verrouillé par les utilisateurs disposant de la permission "Gérer les fils".

Cela empêche toute interaction des autres utilisateurs avec le fil, hormis la lecture des messages.

### Autres options

- **NSFW** : Un fil est configuré comme NSFW (Not Safe For Work) si son salon parent l'est.
  Un message apparaît pour demander à l'utilisateur de confirmer qu'il a bien 18 ans car certaines images/liens/contenus dans le fil peuvent choquer un public non averti.
- **Spoiler** : Si l'option est activée, un message apparaît pour demander à l'utilisateur s'il souhaite voir le contenu du fil, afin de le prévenir qu'il peut contenir des spoilers.
- **Tout le monde peut inviter** : Uniquement disponible pour les fils privés.
  Cette option permet, si désactivée, d'éviter que les utilisateurs autres que le créateur du fil ou des modérateurs puissent ajouter d'autres membres au fil en les mentionnant.
