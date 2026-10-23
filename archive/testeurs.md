---
title: Serveur Discord Testers
keywords:
  - testeur
  - tester
  - bug
  - hunter
  - squasher
  - tracker
  - terminator
description: Le fonctionnement du serveur Discord Testers, la recherche de bugs sur Discord.
contributors: [freiik, dragrame, ben, volcanofr]
short_slug: false
---

:::info L'article est archivé
Le serveur Discord a fermé ses portes, il n'est désormais plus possible de le rejoindre.
Les [badges utilisateurs correspondant](/wiki/compte-utilisateur/personnalisation-profil/badges#bug-hunter), eux, continuent d'exister.
:::

Le [serveur **Discord Testers**](https://discord.gg/discord-testers) est officiel, les employés de l'entreprise le dirigent.
Il sert à réunir toute personne voulant aider à chercher des bugs, failles sur les différents systèmes pour aider le réseau social.
Ces utilisateurs sont souvent appelés par leur nom de tier (exemple: Bug Hunter).
Ils peuvent également faire l'office de test sur de futures nouveautés, qui doivent être testées avant d'être déployées au grand public.

## Tiers {#tiers}

Les tiers permettent d'obtenir des avantages divers.

![Tableau des différents tiers](https://i.dfr.gg/sab.png)

### Tier 1 (`@everyone`) {#tier-1}

Ce tier est disponible à tous les membres lorsqu'ils rejoignent le serveur.

### Tier 2 (Bug Hunter ou Chasseur de bug) {#tier-2}

Le membre doit compléter et passer le « [Bug Hunter Quiz](#quiz) » afin d'accéder à ce tier.
Il débloque les annonces, des salons de discussion avec d'autres chasseurs, ainsi que la possibilité d'[envoyer des bugs](#signalement).

### Tier 3 (Bug Squasher) {#tier-3}

Afin d'accéder à ce tier, l'utilisateur doit avoir trouvé un certain nombre (non divulgué) de bugs approuvés.
La queue d'approbation et un salon de discussion avec les autres chasseurs d'au moins ce tier sont disponibles.

### Tier 4 (Bug Tracker ou Traqueur de bug) {#tier-4}

Ce tier est accessible après avoir réalisé :

* la démonstration de l'utilisation de la queue d'approbation ;
* un certain nombre (non divulgué) de signalements approuvés.

Il débloque les tests de mise au point (Tests Discord Focus) ainsi que [badge Bug Hunter vert](/wiki/compte-utilisateur/personnalisation-profil/badges#bug-hunter).

### Tier 5 (Bug Terminator ou Terminateur de bug) {#tier-5}

Pour accéder à ce tier, il faut :

* maintenir son activité durant une période de 6 mois minimum ;
* avoir un certain nombre (non divulgué) de bugs approuvés **ou** avoir effectué une aide remarquable sur les tests de mise au point.

Ce tier donne le [badge Bug Hunter doré](/wiki/compte-utilisateur/personnalisation-profil/badges#bug-hunter) ainsi que la possibilité de faire partie du groupe junior de modérateurs.

## Bug Hunter Quiz {#quiz}

Le **Quiz** est disponible dans les messages privés de l'application `DBug#8485`, visible en haut de la liste des membres du serveur, en lui envoyant « `!quiz` ».
Il donne un code à usage unique ainsi qu'un lien vers le formulaire.

:::tip
Il est nécessaire pour le membre d'avoir ouvert ses messages privés sur le serveur afin de communiquer avec le bot.
:::

![Accès au formulaire](https://i.dfr.gg/yD2.png)

## Soumission de bug {#signalement}

À partir du [tier 2](#tier-2), il est possible d'envoyer « `!submit` » dans les messages privés du bot `DBug#8485`.

Sinon, il est possible de [**signaler un problème** en créant un ticket de support](https://dfr.gd/bugreport).
