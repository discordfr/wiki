---
title: Expulsion
keywords:
  - expulsion
  - kick
  - expulser
  - modération
  - sanction
  - suppression des membres inactifs
description: L'expulsion, ou kick, est une sanction qui retire un membre d'un serveur tout en lui laissant la possibilité de revenir avec une invitation.
contributors: [zallom, grifgrif]
short_slug: Expulsion
---

L'**expulsion**, appelée *kick* en anglais, est une sanction qui retire un membre d'un serveur.
Le membre expulsé quitte immédiatement le serveur, mais peut le rejoindre à nouveau à l'aide d'une invitation.
Elle se distingue ainsi du [bannissement](/wiki/gestion-serveur/moderation/bans), qui empêche tout retour, et de l'[exclusion temporaire](/wiki/gestion-serveur/moderation/timeout), qui laisse le membre sur le serveur en limitant ses interactions.

:::note Vocabulaire
Dans l'interface française de Discord, l'expulsion correspond à l'action « Expulser ». L'action « Exclure » désigne l'[exclusion temporaire](/wiki/gestion-serveur/moderation/timeout), souvent appelée *timeout* pour éviter la confusion.
:::

## Fonctionnement {#fonctionnement}

Lorsqu'un membre est expulsé, le serveur disparaît de sa liste de serveurs. Discord lui envoie un message privé depuis son compte système : « Un modérateur du serveur t'a retiré(e) de [nom du serveur]. Discord n'a pas pris cette décision de modération. » Ce message est identique pour un [bannissement](/wiki/gestion-serveur/moderation/bans), et la raison n'y figure pas.
Rien ne l'empêche ensuite de revenir : il peut rejoindre le serveur dès qu'il dispose d'une invitation valide, y compris immédiatement après son expulsion.

Les messages envoyés par le membre avant son expulsion restent sur le serveur : l'expulsion ne comporte aucune option de suppression des messages.

L'expulsion est enregistrée dans les [logs du serveur](/wiki/gestion-serveur/moderation/logs), avec le modérateur à l'origine de l'action et, le cas échéant, la raison indiquée.

## Permission requise {#permission}

L'expulsion nécessite la permission « [Expulser, accepter et refuser des membres](/wiki/gestion-serveur/permissions/membres) » (`KICK_MEMBERS` dans l'API).
Cette même permission permet d'accepter ou de refuser les demandes d'adhésion sur les serveurs qui imposent une candidature pour les rejoindre.
Lorsque le serveur exige l'[authentification à deux facteurs](/wiki/compte-utilisateur/authentification/a2f) (A2F) pour les actions de modération, cette permission n'est utilisable que par les membres ayant activé l'A2F.

L'expulsion respecte la hiérarchie des rôles : un membre ou une application (bot) ne peut expulser que les membres dont le rôle le plus haut se situe en dessous de son propre rôle le plus haut.
Le propriétaire du serveur n'est pas soumis à cette limite et ne peut pas être expulsé. <!-- À VÉRIFIER : aucune source officielle trouvée pour le cas du propriétaire -->

## Expulsion d'un membre {#expulser}

Sur ordinateur, l'expulsion se fait depuis le menu contextuel du membre :

1. Effectuer un clic droit sur le pseudo du membre, dans un message ou dans la liste des membres.
2. Cliquer sur « Expulser » suivi du pseudo du membre.
3. Dans la fenêtre de confirmation, le modérateur peut indiquer une raison.
4. Cliquer sur « Expulser ».

Sur mobile, l'expulsion se fait depuis le profil du membre :

1. Appuyer sur le pseudo ou l'avatar du membre, dans un message ou dans la liste des membres.
2. Appuyer sur « Expulser », directement dans le profil.
3. Indiquer éventuellement une raison, puis confirmer l'expulsion.

<!-- TODO: capture anonyme du menu contextuel d'un membre sur ordinateur, avec l'option « Expulser » mise en évidence (aucun pseudo ni avatar réel visible) -->
<!-- TODO: capture anonyme de la fenêtre de confirmation de l'expulsion, avec le champ de raison -->

Les applications disposant de la permission peuvent également expulser des membres par l'intermédiaire de l'API, généralement à l'aide d'une commande ou d'une règle de modération automatique.

## Suppression des membres inactifs {#prune}

La suppression des membres inactifs (*prune*), appelée « Congédier » dans l'interface française, est une expulsion groupée des membres qui ne se sont pas connectés depuis une durée donnée.
La durée d'inactivité peut être fixée à 7 ou 30 jours. Par défaut, seuls les membres sans rôle sont concernés ; une option permet d'inclure les membres de certains rôles.
Elle nécessite, en plus de la permission d'expulsion, la permission « Gérer le serveur » (`MANAGE_GUILD`).

## Conséquences pour le membre {#consequences}

### Rôles {#roles}

En quittant le serveur, le membre perd l'ensemble des rôles qu'il possédait.
S'il revient, il rejoint le serveur comme un nouveau membre, sans ses rôles précédents.

Cette perte concerne aussi les rôles attribués par des applications de niveaux (*leveling*), qui récompensent l'activité des membres sur le serveur : le membre expulsé perd ainsi les rôles qui reflètent son niveau.
La restitution de ces rôles à son retour dépend du fonctionnement de l'application.

Certaines applications proposent des **rôles persistants** : elles enregistrent les rôles d'un membre lorsqu'il quitte le serveur et les lui rendent lorsqu'il revient.
Ce mécanisme n'est pas natif.
Les rôles rendus par un tel système sont ceux que le membre possédait au moment de son départ.

### Boosts {#boosts}

Un membre qui [boostait](/wiki/contenu-payant/boost-serveur) le serveur perd ses boosts sur celui-ci lorsqu'il en est retiré. Ses boosts sont soumis à un délai de recharge de 7 jours avant de pouvoir être réutilisés, et sa série de boost peut être perdue s'ils ne sont pas réappliqués à un autre serveur dans les 72 heures.

## Comparaison avec les autres sanctions {#comparaison}

| Sanction | Libellé dans l'interface | Le membre reste sur le serveur | Retour possible |
| --- | --- | --- | --- |
| Expulsion (*kick*) | « Expulser » | Non | Oui, avec une invitation |
| [Exclusion temporaire](/wiki/gestion-serveur/moderation/timeout) (*timeout*) | « Exclure » | Oui, en lecture seule | Sans objet |
| [Bannissement](/wiki/gestion-serveur/moderation/bans) (*ban*) | « Bannir » | Non | Non, sauf débannissement |

## Usages courants {#usages}

Sur les serveurs, l'expulsion est notamment employée dans les situations suivantes :

- **Compte piraté** : un compte compromis qui envoie du spam est retiré du serveur, et son propriétaire légitime peut revenir une fois le compte récupéré ;
- **Profil inapproprié** : un compte dont le profil (avatar, bannière, biographie, pseudo) ne correspond pas aux règles du serveur, par exemple un profil à caractère sexuel, est retiré, avec la possibilité de revenir après modification de ce profil.

Dans ces cas, l'expulsion retire le membre du serveur sans le bannir : il peut revenir une fois la situation corrigée.
D'autres serveurs utilisent à la place un rôle d'isolement, attribué par une application, qui retire au membre l'accès aux salons sans lui faire quitter le serveur.
