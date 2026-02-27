---
title: Salons de conférence
keywords:
  - serveur
  - vocal
  - conférence
  - stage
  - salon
  - channel
description: Les Stage Channels, le système de conférence de Discord avec intervenants et auditeurs.
contributors: [ichii, luke, wolfyzdbois, volcanofr]
---

Les **Stage Channels** sont des salons vocaux permettant des conférences : un nombre restreint d'intervenants sélectionnés s'expriment devant une audience.

:::note
Cette fonctionnalité n'est disponible que sur les serveurs ayant [activé la communauté](/wiki/gestion-serveur/outils-communautaires#activer-le-serveur-communautaire).
:::

## Fonctionnement des Stage Channels

Étant basés sur les salons vocaux classiques, leur fonctionnement est très similaire.
Il est possible pour l'utilisateur de se rendre muet, et de couper son micro normalement.
Les présentateurs peuvent aussi utiliser la fonctionnalité [Go Live](/wiki/interface/salons-vocaux/partage-video) pour streamer en direct et activer leur caméra.

Comme différence notable, seuls les intervenants sont affichés séparément des autres utilisateurs présents dans le salon.
Les auditeurs peuvent uniquement prendre la parole quand un modérateur leur propose, ou qu'ils sont acceptés par un modérateur après avoir demander à prendre la parole.

Lorsque tous les intervenants ont coupé leur micro, Discord diffuse automatiquement une musique d'attente aux utilisateurs présents ne l'ayant pas désactivé.

![Interfarce en étant dans un salon de conférence](https://i.dfr.gg/Ynus.png)

:::note
Comme dans tous les salons vocaux, la [suppression des bruits de fond](/wiki/interface/salons-vocaux/krisp) n'est pas activée par défaut pour les intervenants.
:::

### La modération

Les utilisateurs ayant la permission de déplacer, de rendre muet des membres et de gérer le salon ont la possibilité de modérer la présentation à leur guise.
Ces derniers ont la possibilité d'effectuer les actions suivantes :

- Changer leur place de l'audience aux présentateurs directement.
- Déplacer les membres des présentateurs à l'audience et inviter des membres de l'audience à parler.
- Voir les demandes de prise de parole.

![Les demandes de parole](https://i.dfr.gg/DemandesParole.webp)

De plus, pour être facilement reconnaissables, les modérateurs possèdent une icône notifiant les utilisateurs de leurs permissions.

![Les présentateurs & Modérateurs](https://i.dfr.gg/PresentateursModerateurs.webp)

### L'audience

Lorsque la présentation est ouverte, n'importe quel membre ayant accès au salon a la possibilité d'y assister.
Une icône à côté du bouton fait pour quitter le salon permet de demander la parole auprès des modérateurs, qui disposent de la possibilité d'approuver ou de rejeter cette requête.

### Limite d'utilisateur

Sans utilisation de la caméra ni du partage d'écran, jusqu'à 10 000 membres peuvent être présents dans l'audience.

Si un intervenant utilise sa caméra ou fait un partage d'écran, la limite dépend du niveau de boosts du serveur :
- 50 utilisateurs présents par défaut dans le salon.
- 150 utilisateurs si le serveur est niveau 2.
- 300 utilisateurs si le serveur est niveau 3.
- Puis la limite augmente de 30 utilisateurs par boost jusqu'à une limite de 10 000 utilisateurs, présentateurs et audience compris.

## Informations complémentaires

- Lors de l'activation d'un Stage Channel, il devient vert et une notification apparaît en haut du serveur pour notifier de la présence d'une présentation.
- Un sujet doit être ajoutée au salon et sera affichée directement en dessous de son nom pour donner une courte description de la discussion.
- Jusqu'à 5 personnes en conférence peuvent activer leurs caméras et faire un partage d'écran en simultané.
- Les membres présents dans une conférence en cours reçoivent un statut l'indiquant.

![Pop-up Stage](https://i.dfr.gg/Pop-upStage.webp)
