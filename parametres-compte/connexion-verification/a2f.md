---
id: a2f
title: L'authentification à deux facteurs
keywords:
  - discord
  - a2f
  - authentification
  - tutoriel
  - compte
  - sécurité
description: Utilisation de l'authentification à deux facteurs sur Discord
---

## Le principe
L'authentification à deux facteurs, ou A2F, est un système servant à apporter une couche de sécurité supplémentaire à un compte en ligne. C'est-à-dire : avoir deux facteurs différents requis pour s'authentifier. Sur Discord le mot de passe et un code renouvelé régulièrement grâce à une application mobile seraient requis pour accéder à un compte. Ce code d'authentification est généré toutes les 30 secondes et déverrouille le compte après avoir rentré le mot de passe.

:::info
La fonctionnalité de [QR Code](https://discord.fr/wiki/parametres-compte/connexion-verification/qr-code.md) passera toujours outre l'authentification à deux facteurs.
:::

## Codes de secours
Lors de l'activation de l'A2F, Discord génère des codes de secours générés aléatoirement. Dans le cas où l' utilisateur perd son application d'authentification, il sera alors possible d'utiliser un de ces codes au lieu de l'A2F pour se connecter au compte.

:::caution
Discord ne génèrera jamais de codes de secours ou ne désactivera l'A2F d'un compte sous aucun prétexte et ce même sur demande explicite de l'utilisateur.
:::

## Quel programme choisir pour l'A2F ?
Il est recommandé d'utiliser des services reconnus, comme [Authy](https://authy.com/), disponible sous presque tous les systèmes d'exploitation (Smartphone, macOS et Windows) ou bien Google Authenticator, disponible sous [Android](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2) et [iOS](https://apps.apple.com/us/app/google-authenticator/id388497605).

## Références 
[Guide d'activation de l'A2F](https://discord.fr/blog/2021/02/25/double-authentification/)
