---
title: Les Salons de Conférence
keywords:
  - discord
  - serveur
  - vocal
  - conférence
  - stage channels
description: Les Stage Channels sur Discord
contributors: [ichii, luke]
---

Les **Stage Channels** sont des salons vocaux spéciaux permettant à un nombre limité d'utilisateurs de parler tandis qu'un plus grand nombre d'auditeurs peuvent être présents à les écouter. 

## Le fonctionnement des Stage Channels

Étant basés sur les salons vocaux classiques, leur fonctionnement est très similaire. Il est possible pour l'utilisateur de se rendre muet, et de couper son micro normalement. La seule différence notable étant que seuls les présentateurs sont affichés séparément des autres utilisateurs sur le serveur et que les auditeurs n'ont pas le droit de prendre la parole à moins que les modérateurs de la présentation la leur accordent.

Par ailleurs, les présentateurs peuvent utiliser la fonctionnalité [Go Live](/wiki/interface/salons-vocaux/partage-video) pour streamer en direct et activer leur caméra.

:::note::: À noter
Lorsqu'une session n'a pas encore été débutée, Discord diffuse automatiquement une musique d'attente dans le stage channel. 
:::

![L'affichage des présentateurs](https://i.dfr.gg/AffichagePresentateurs.webp)

### La modération
Les utilisateurs ayant la permission de déplacer, de rendre muet des membres et de gérer le salon, ont la possibilité de modérer la présentation à leur guise.
Ces derniers ont la possibilité d'effectuer les actions suivantes :

- Changer leur place de l'audience aux présentateurs directement.
- Déplacer les membres des présentateurs à l'audience et inviter des membres de l'audience à parler.
- Voir les demandes de prise de parole.

![Les demandes de parole](https://i.dfr.gg/DemandesParole.webp)

De plus, pour être facilement reconnaissables, les modérateurs possèdent une icône notifiant les utilisateurs de leurs permissions.

![Les présentateurs & Modérateurs](https://i.dfr.gg/PresentateursModerateurs.webp)

### L'audience

Lorsque la présentation est ouverte, n'importe quel membre du serveur a la possibilité d'y assister. Les membres sont séparés en fonction de leurs rôles, si ces derniers sont affichés séparément des autres. Une icône à côté du bouton fait pour quitter le salon permet de demander la parole auprès des modérateurs, qui disposent de la possibilité d'approuver ou de rejeter cette requête.

### Le Stage Discovery

Le Stage Discovery permet aux stage channels d'être référencés publiquement, et par conséquent d'être rejoints par n'importe quel utilisateur de Discord. Cette option n'est toutefois pas disponible pour n'importe quel stage channel.

Pour utiliser le Stage Discovery, il faut activer le référencement au début d'une conférence. Le salon en question doit être accessible au rôle `@everyone`.

![Stage Discovery](https://i.dfr.gg/frZ.png)

## Informations Complémentaires
- Lors de l'activation d'un Stage Channel, il devient vert et une notification apparaît en haut du serveur pour notifier de la présence d'une présentation.
- Une description peut-être ajoutée au salon et sera affichée directement en dessous de son nom pour donner le thème de la discussion.
- La limite de membres présents simultanément dans le salon est de 1000 utilisateurs, présentateurs et audience compris.

![Pop-up Stage](https://i.dfr.gg/Pop-upStage.webp)
