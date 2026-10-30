---
title: Authentification par SMS
keywords:
  - sms
  - téléphone
  - telephone
  - connexion
  - compte
description: S'authentifier par SMS (SMS Auth) sur Discord, la fonctionnalité de secours.
contributors: [mapidae]
short_slug: false
---

L'**authentification par SMS** est une méthode courante utilisée pour renforcer la sécurité des comptes.
Elle consiste à recevoir un code de vérification envoyé via un message texte sur un numéro de téléphone associé au compte utilisateur.

## Fonctionnement

Lorsqu'un utilisateur active l'authentification par SMS, le service envoie un **code à usage unique** sur le numéro de téléphone enregistré.
Ce code doit être saisi dans l'interface pour valider l'authentification.
Cette méthode est souvent utilisée comme mesure de sécurité supplémentaire pour vérifier l'identité de l'utilisateur lors de la connexion à un compte en ligne.

## Utilisation dans Discord

Les utilisateurs peuvent associer leur numéro de téléphone à leur compte Discord pour recevoir un code de vérification par SMS lors de la connexion depuis un nouvel appareil ou lors de la configuration de l'[authentification à deux facteurs](/wiki/compte-utilisateur/authentification/a2f).

## Préoccupations de sécurité

Bien que l'authentification par SMS offre une couche supplémentaire de sécurité, elle présente des **risques potentiels**.
Les attaques telles que le SIM Swap, où un attaquant vole la carte SIM d'un utilisateur, peuvent compromettre cette méthode d'authentification.
Les SMS peuvent également être interceptés, compromettant ainsi la sécurité du compte.

:::warning
L'authentification par SMS est généralement déconseillée, en particulier sans un contrôle total sur la ligne téléphonique.
Des services tels que OnOff peuvent constituer une option plus fiable pour ceux qui préfèrent disposer d'une ligne secondaire spécifiquement dédiée à l'authentification, éliminant ainsi les risques d'interception de messages via des méthodes spécifiques.
:::

:::note
En France, où la protection des données est un enjeu majeur, les opérateurs mobiles peuvent être vulnérables aux techniques d'ingénierie sociale, permettant ainsi l'utilisation frauduleuse de numéros.
Cependant, les opérateurs mobiles ne sont pas les seules victimes de telles pratiques.
:::

---

:::info L'article nécessite des modifications
* Rattacher l'article à Discord plutôt que faire une généralisation ;
* Mettre à jour l'article : l'[A2F](/wiki/compte-utilisateur/authentification/a2f) est requis pour configurer le téléphone.

Ce projet communautaire vise à offrir un contenu librement réutilisable, que chacun peut modifier et améliorer.
Pour contribuer, munissez-vous d'un compte GitHub et rendez-vous sur notre [page de contribution](/wiki/contribuer).
:::
