---
title: Bannissement
keywords:
  - bannissement
  - ban
  - débannissement
  - liste des bannissements
  - modération
  - adresse IP
description: Le bannissement retire un utilisateur d'un serveur et l'empêche d'y revenir tant que la sanction n'est pas révoquée depuis la liste des bannissements.
contributors: [zallom, grifgrif]
short_slug: Bannissement
---

Le **bannissement**, appelé *ban* en anglais, est une sanction qui retire un utilisateur d'un serveur et l'empêche de le rejoindre à nouveau.
Il se distingue de l'[expulsion](/wiki/gestion-serveur/moderation/expulsion), après laquelle l'utilisateur peut revenir avec une invitation, et de l'[exclusion temporaire](/wiki/gestion-serveur/moderation/timeout), qui le laisse sur le serveur.
Les utilisateurs bannis sont répertoriés dans la **[liste des bannissements](#liste)**, depuis laquelle un bannissement peut être révoqué.

## Fonctionnement {#fonctionnement}

Un utilisateur banni est retiré du serveur et ne peut plus le rejoindre avec ce compte.
Discord ne propose pas de durée de bannissement : la sanction s'applique jusqu'à ce qu'un membre autorisé la révoque.
Les bannissements temporaires proposés par certaines applications (bots) reposent sur une révocation automatique effectuée par l'application à la fin de la durée choisie.

Le membre qui bannit un utilisateur peut indiquer une raison.
Celle-ci est visible par les membres qui ont accès à la liste des bannissements et apparaît dans les [logs du serveur](/wiki/gestion-serveur/moderation/logs), où sont consignés les bannissements et les débannissements.

### Permissions requises {#permissions}

Bannir un utilisateur nécessite la permission « [Bannir des membres](/wiki/gestion-serveur/permissions/membres) ».
Un membre ne peut pas bannir un utilisateur dont le rôle le plus haut est égal ou supérieur au sien, même s'il dispose de cette permission.
Le propriétaire du serveur ne peut pas être banni.
Si le serveur exige l'[authentification à deux facteurs](/wiki/compte-utilisateur/authentification/a2f) (A2F) pour les actions de modération, cette permission ne peut être utilisée que par un membre dont le compte a activé l'A2F.

### Bannissement d'un membre {#bannir}

Sur ordinateur et sur navigateur :

1. Effectuer un clic droit sur le pseudo du membre, dans un message ou dans la liste des membres.
2. Cliquer sur « Bannir » suivi du pseudo du membre.
3. Indiquer, si besoin, une raison et choisir dans « Supprimer l'historique des messages » la période des messages à supprimer.
4. Cliquer sur « Bannir ».

Sur mobile :

1. Appuyer sur l'avatar du membre pour afficher son profil.
2. Appuyer sur « Bannir ».
3. Indiquer, si besoin, une raison et confirmer.

![Fenêtre de banissement d'un membre](https://i.dfr.gg/FpAt.png)

### Bannissement multiple {#bannissement-multiple}

La page « Membres » du serveur permet de bannir plusieurs utilisateurs à la fois, en cochant la case située à gauche de chacun d'eux.
Ce bannissement multiple nécessite à la fois la permission « Gérer le serveur » et la permission « Bannir des membres ».
Pour des raisons de sécurité, Discord demande au membre qui l'effectue de saisir son code A2F ou son mot de passe.
Par l'intermédiaire de l'API, une application peut bannir jusqu'à 200 utilisateurs en une seule requête.

### Suppression des messages récents {#suppression-messages}

Au moment du bannissement, Discord permet de supprimer les messages envoyés récemment par l'utilisateur sur le serveur.
L'option « Supprimer l'historique des messages » propose de ne rien supprimer, ou de supprimer les messages de la dernière heure, des 6, 12 ou 24 dernières heures, des 3 ou des 7 derniers jours.
Par l'intermédiaire de l'API, la période s'exprime en secondes, de 0 à 604 800 (soit 7 jours).

## Liste des bannissements {#liste}

La liste des bannissements se trouve dans « Paramètres du serveur » > « Bannissements ».
Elle répertorie tous les utilisateurs bannis du serveur et permet de rechercher un utilisateur par son nom ou son identifiant.
Lorsqu'un utilisateur est sélectionné, la raison de son bannissement s'affiche, si une raison a été indiquée.

Par l'intermédiaire de l'API, la liste est accessible aux applications disposant de la permission « Bannir des membres » ou « Voir les logs du serveur », par pages de 1 000 utilisateurs au maximum.

![Liste des bannissements d'un serveur](https://i.dfr.gg/za8R.png)

### Débannissement {#debannissement}

Le débannissement (ou révocation du bannissement) s'effectue depuis la liste des bannissements, en sélectionnant l'utilisateur puis le bouton « Révoquer le bannissement ».
L'utilisateur n'est pas réintégré au serveur : il peut seulement le rejoindre à nouveau avec une invitation.

## Conséquences pour l'utilisateur banni {#consequences}

### Ce que voit l'utilisateur {#affichage}

Le serveur disparaît de la liste des serveurs de l'utilisateur banni.
Discord lui envoie un message privé depuis son compte système : « Un modérateur du serveur t'a retiré(e) de [nom du serveur]. Discord n'a pas pris cette décision de modération. »
Ce message est identique pour une [expulsion](/wiki/gestion-serveur/moderation/expulsion).
Discord ne lui communique pas la raison du bannissement.
Certaines applications envoient un message privé à l'utilisateur pour l'informer de la sanction ; ce fonctionnement n'est pas natif.

Lorsque l'utilisateur banni tente d'utiliser une invitation vers le serveur, Discord affiche « Invitation invalide », suivi de « L'utilisateur est banni de ce serveur ».

### Boosts {#boosts}

Un utilisateur qui [boostait](/wiki/contenu-payant/boost-serveur) le serveur perd ses boosts sur celui-ci lorsqu'il en est retiré.
Ses boosts sont soumis à un délai de recharge de 7 jours avant de pouvoir être réutilisés, et sa série de boost peut être perdue s'ils ne sont pas réappliqués à un autre serveur dans les 72 heures.

### Messages privés {#messages-prives}

Le bannissement ne supprime pas les conversations privées existantes entre l'utilisateur banni et les membres du serveur.
Un utilisateur ne peut toutefois écrire à un autre que s'ils sont amis ou s'ils partagent un serveur où ce dernier accepte les messages privés des membres.
Sans autre serveur en commun, l'utilisateur banni ne peut donc plus écrire qu'à ses amis, y compris dans une conversation déjà ouverte.
S'il partage encore un autre serveur avec un membre, il peut continuer à lui écrire.

## Bannissement d'une adresse IP {#adresse-ip}

D'après le centre d'aide de Discord, « Les bannissements de serveur sont basés sur les adresses IP ».
Une adresse IP est l'identifiant attribué à une connexion à internet.
Discord ne documente pas davantage ce fonctionnement.

Discord pourrait également tenir compte de l'appareil utilisé.
Les autres comptes de l'utilisateur déjà présents sur le serveur au moment du bannissement ne sont pas affectés.

:::note Adresses IPv4 partagées
En raison de la pénurie d'adresses IPv4, le format d'adresse IP le plus répandu, certains opérateurs attribuent une même adresse à de nombreux abonnés, y compris sur les réseaux mobiles (4G et 5G).
Ce partage entraîne des faux positifs : des utilisateurs sans lien avec le compte banni ne peuvent pas rejoindre le serveur.
:::

## Comparaison avec les autres sanctions {#comparaison}

| Sanction | Libellé dans l'interface | Le membre reste sur le serveur | Retour possible |
| --- | --- | --- | --- |
| [Exclusion temporaire](/wiki/gestion-serveur/moderation/timeout) (*timeout*) | « Exclure » | Oui, en lecture seule | Sans objet |
| [Expulsion](/wiki/gestion-serveur/moderation/expulsion) (*kick*) | « Expulser » | Non | Oui, avec une invitation |
| Bannissement (*ban*) | « Bannir » | Non | Non, sauf débannissement |

## Usages courants {#usages}

Sur les serveurs, le bannissement est notamment employé dans les situations suivantes :

* **Compte malveillant** : un compte venu pour nuire, par exemple lors d'un raid ou d'une tentative d'arnaque ;
* **Récidive** : un membre qui a déjà reçu des avertissements ou d'autres sanctions, restés sans effet ;
* **Softban** : un bannissement suivi d'un débannissement immédiat, qui supprime les messages récents du compte sans l'empêcher de revenir avec une invitation.

D'autres serveurs utilisent à la place un rôle d'isolement, attribué par une application, qui retire au membre l'accès aux salons sans lui faire quitter le serveur.
Discord FR déconseille le bannissement dans la plupart des cas et recommande cet isolement, pour les raisons détaillées dans l'article « [Bannir les membres de son serveur : une solution obsolète ?](/blog/2026/10/19/ban-discord-solution-obsolete) ».
