---
title: Mode développeur
keywords:
  - dev
  - développeur
  - identifiant
  - copier
  - mode
  - api
  - activité
description: Le mode développeur sur Discord permet de copier les différents identifiants.
contributors: [moonrise, volcanofr]
---

Le mode développeur permet d'activer des **options supplémentaires** sur Discord.
L'intérêt principal de l'activer est de pouvoir récupérer l'identifiant (ID) d'un utilisateur, d'un message, d'un serveur, etc.

## Activation

Le mode développeur est activable pour tous les utilisateurs Discord dans les **paramètres d'utilisateur**, section **Développeur** sur ordinateur et **Avancés** sur mobile.

![Bouton d'activation du mode développeur](https://i.dfr.gg/KOto.png)

## Fonctionnalités

Une fois le mode activé, des options supplémentaires peuvent apparaître dans certains menus.

### Copie d'identifiant

En cliquant droit sur un nom d'utilisateur, sur l'icône d'un serveur, au-dessus d'un message, et d'autres endroits de l'interface, il est possible de copier l'identifiant correspondant à la fonctionnalité visée.

![Copie de l'identifiant d'une commande](https://i.dfr.gg/O374.png)

Il est possible de copier l'identifiant des éléments suivants :

* [Utilisateur](/wiki/compte-utilisateur) et application (bot)
* [Serveur](/wiki/gestion-serveur)
* Salon (comprenant les [messages privés](/wiki/interface/appel-message-prives)) et catégorie
* Message et pièce jointe
* [Émoji](/wiki/interface/salons-textuels/emojis-reactions), autocollant et soundboard
* Commande
* [Rôle](/wiki/gestion-serveur/configuration/roles)
* [Événement](/wiki/gestion-serveur/outils-communautaires/events)
* Quête
* Règle d'AutoMod
<!-- * Jeu et SKU (Apparaît dans les strings, mais n'est pas utilisé in-app) -->
<!-- * Récurrence (Apparaît dans les strings, mais n'est pas utilisé in-app) -->
<!-- * Tag (Apparaît dans les strings, mais n'est pas utilisé in-app) -->

L'identifiant (ID) est aussi appelé "Snowflake" par les développeurs.
D'autres identifiants existent au travers de l'[API Discord](https://docs.discord.com/developers/reference#snowflakes), mais ils ne peuvent pas être copiés dans l'application Discord.

### Mode de test d'application

Dans les paramètres utilisateur au même emplacement que l'[activation du mode développeur](#activation), l'utilisateur peut activer le **Mode de test d'application**.

Cette option permet aux développeurs et testeurs de tester une activité, liée à une application Discord.

Dans les [salons textuels](/wiki/interface/salons-textuels), l'activité liée est alors disponible aux utilisateurs concernés dans la liste de lancement d'applications.
Elle est aussi accessible depuis l'étagère des activités des développeurs dans les [salons vocaux](/wiki/interface/salons-vocaux).

### Dérogation d'URL d'activité

Disponible depuis l'étagère des activités des développeurs des salons vocaux, il est possible de forcer l'[URL de base](https://developer.mozilla.org/docs/Web/API/Node/baseURI) de toutes les requêtes `HTTP` faites par l'**activité** lancée par l'utilisateur.
Toutes les informations, qui communiquent habituellement entre le serveur de l'activité et l'application, passent alors sur l'addresse renseignée.
