---
title: Exclusion temporaire
keywords:
  - exclusion temporaire
  - timeout
  - exclure
  - sanction
  - modération
description: L'exclusion temporaire, ou timeout, est une sanction native de Discord qui empêche un membre d'interagir avec un serveur pendant une durée déterminée, sans le retirer du serveur.
contributors: [zallom, grifgrif]
short_slug: ExclusionTemporaire
---

L'**exclusion temporaire**, appelée *timeout* en anglais, est une sanction native de Discord qui empêche un membre d'interagir avec un serveur pendant une durée déterminée.
Le membre n'est pas retiré du serveur : il peut toujours lire les salons, mais ne peut plus y envoyer de messages, ajouter de nouvelles réactions ni rejoindre de salon vocal.
Elle se distingue ainsi de l'[expulsion](/wiki/gestion-serveur/moderation/expulsion) et du [bannissement](/wiki/gestion-serveur/moderation/bans), qui retirent le membre du serveur.
L'exclusion temporaire prend fin automatiquement à l'expiration de la durée choisie, ou plus tôt si un modérateur la lève.

La fonctionnalité a été introduite en décembre 2021.
Elle est réservée aux membres disposant de la permission « [Exclure temporairement des membres](/wiki/gestion-serveur/permissions/membres) ».

:::note
Dans l'interface française de Discord, l'action d'exclusion temporaire s'intitule « Exclure », alors que l'action qui retire un membre du serveur s'intitule « Expulser ».
Les deux mots étant proches, le terme anglais *timeout* est couramment employé par les utilisateurs francophones pour désigner l'exclusion temporaire et éviter la confusion avec l'[expulsion](/wiki/gestion-serveur/moderation/expulsion).
:::

## Fonctionnement {#fonctionnement}

Pendant une exclusion temporaire, le membre perd toutes ses permissions sur le serveur, à l'exception de « Voir les salons » et « Voir les anciens messages ».
Cette restriction s'applique à l'ensemble des salons du serveur : il n'est pas possible d'exclure temporairement un membre d'un seul salon.

Le propriétaire du serveur et les membres disposant de la permission « Administrateur » ne peuvent pas être exclus temporairement.
Un modérateur ne peut exclure temporairement qu'un membre dont le rôle le plus haut se situe strictement en dessous du sien : un membre de rang égal ou supérieur ne peut pas être exclu.

L'exclusion temporaire ne modifie pas les rôles du membre.
Comme elle ne retire pas le membre du serveur, les [boosts](/wiki/contenu-payant/boost-serveur) qu'il a attribués au serveur sont conservés.

## Durées {#durees}

L'interface de Discord propose six durées :

* 60 secondes ;
* 5 minutes ;
* 10 minutes ;
* 1 heure ;
* 1 jour ;
* 1 semaine.

Les applications (bots) peuvent appliquer une durée personnalisée, jusqu'à 28 jours (voir [AutoMod et applications](#applications)).

## Application d'une exclusion temporaire {#application}

L'exclusion temporaire s'applique depuis le menu contextuel du membre sur ordinateur, ou depuis son profil sur mobile.
Le modérateur choisit la durée et peut indiquer une raison.

Sur ordinateur et sur navigateur :

1. Effectuer un clic droit sur le pseudo du membre, dans un message ou dans la liste des membres.
2. Cliquer sur « Exclure ».
3. Choisir la durée et, le cas échéant, indiquer la raison.
4. Cliquer sur « Exclure temporairement ».

Sur mobile :

1. Appuyer sur l'avatar du membre pour afficher son profil.
2. Appuyer sur « Exclure temporairement ».
3. Choisir la durée et confirmer.

![Fenêtre d'exclusion d'un membre](https://i.dfr.gg/8EVm.png)

## Effets pour le membre exclu {#effets}

Pendant toute la durée de l'exclusion temporaire, le membre :

* peut lire les salons et consulter leurs anciens messages ;
* voit un compte à rebours indiquant le temps restant avant la fin de la sanction ;
* ne peut pas envoyer de messages ;
* ne peut pas ajouter de nouvelle réaction, mais peut ajouter la sienne à une réaction déjà présente sur un message ;
* ne peut pas rejoindre de salon vocal ;
* ne peut pas utiliser les boutons et les autres composants des messages, comme ceux qui servent à ouvrir un ticket, ni les commandes des applications.

La raison saisie par le modérateur n'est pas affichée au membre exclu.

L'exclusion temporaire ne bloque pas les messages privés (MP) : le membre exclu peut toujours écrire aux autres membres du serveur, dans les conditions habituelles.

![Salon vu par un membre exclu temporairement](https://i.dfr.gg/c1qo.png)

## Visibilité pour la modération {#visibilite}

Les membres disposant de la permission « Exclure temporairement des membres » voient une icône à côté de l'horodatage des messages d'un membre exclu.
Les autres membres du serveur voient ces messages sans changement.

La page « Membres » du serveur, disponible sur navigateur et sur ordinateur, propose un filtre « Exclu temporairement » qui affiche les membres actuellement exclus.
Sur un serveur Communauté, cette page est accessible depuis la liste des salons ; sur les autres serveurs, elle se trouve dans « Paramètres du serveur » > « Membres ».

Chaque exclusion temporaire, avec sa durée et sa raison, est consignée dans les [logs du serveur](/wiki/gestion-serveur/moderation/logs).

## Levée d'une exclusion temporaire {#levee}

Une exclusion temporaire peut être levée avant la fin de la durée prévue par un membre disposant de la permission « Exclure temporairement des membres ».

Sur ordinateur et sur navigateur :

1. Effectuer un clic droit sur le pseudo du membre, dans un message ou dans la liste des membres.
2. Cliquer sur « Arrêter d'exclure » suivi du pseudo du membre.
3. Confirmer la suppression.

Sur mobile :

1. Appuyer sur l'avatar du membre pour afficher son profil.
2. Appuyer sur « Arrêter d'exclure ».
3. Confirmer la suppression.

## AutoMod et applications {#applications}

L'AutoMod, l'outil de modération automatique intégré à Discord, peut appliquer une exclusion temporaire au membre dont un message déclenche l'une de ses règles.
Cette action n'est disponible que pour les règles de mots-clés et de spam de mentions. Elle propose les mêmes durées que l'interface, sans durée personnalisée.

Les applications peuvent appliquer, modifier ou lever une exclusion temporaire par l'intermédiaire de l'API de Discord, pour une durée de 28 jours au maximum.
Elles doivent pour cela disposer de la permission « Exclure temporairement des membres », désignée par la constante `MODERATE_MEMBERS` dans l'API.

## Comparaison avec les autres sanctions {#comparaison}

| Sanction | Libellé dans l'interface | Le membre reste sur le serveur | Retour possible |
| --- | --- | --- | --- |
| Exclusion temporaire (*timeout*) | « Exclure » | Oui, en lecture seule | Sans objet |
| [Expulsion](/wiki/gestion-serveur/moderation/expulsion) (*kick*) | « Expulser » | Non | Oui, avec une invitation |
| [Bannissement](/wiki/gestion-serveur/moderation/bans) (*ban*) | « Bannir » | Non | Non, sauf débannissement |

## Usages courants {#usages}

Sur les serveurs, l'exclusion temporaire est notamment employée dans les situations suivantes :

* **Échange qui s'envenime** : une dispute ou un débat houleux, le temps que la tension retombe ;
* **Spam** : un membre qui envoie des messages en rafale ou mentionne en masse d'autres membres, souvent sanctionné automatiquement par l'AutoMod ;
* **Sanction graduée** : une étape intermédiaire avant l'expulsion ou le bannissement, en cas de récidive ;
* **Compte suspect** : un compte qui semble piraté, le temps de vérifier la situation sans le retirer du serveur.
