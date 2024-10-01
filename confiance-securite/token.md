---
title: Token
keywords:
  - discord
  - token
description: Token
contributors: [mapidae]
short_slug: Tokens
---

Un token Discord est une chaîne de caractères unique qui agit comme une forme d'authentification directe et qui permet de communiquer avec les services internes de Discord (l’API). En d'autres termes, le token est une sorte de clé d'accès qui permet à l'application de se connecter à Discord et d'interagir avec ses fonctionnalités.
Si un message est envoyé sur Discord : le token est sollicité pour envoyer l’information.

Chaque bot ou compte requiert un token pour être autorisé à fonctionner sur la plateforme. Ils sont générés par Discord et sont composés de moitié à partir de votre identifiant unique Discord. Donc pas de panique si un utilisateur vous partage le début de votre token !

Il est crucial de traiter les tokens avec beaucoup de précautions, car quiconque a accès à un token Discord peut contrôler le bot ou le compte associé. 
En ce qui concerne les bots, les tokens ne doivent jamais être partagés publiquement ou inclus dans du code source accessible par d'autres utilisateurs, car cela pourrait compromettre la sécurité du bot. 

## Comment changer son token ?

En cas de compromission d'un token, il est recommandé de le réinitialiser immédiatement pour éviter tout accès non autorisé au bot. 
Pour changer le token d’un compte il suffit de se rendre dans les paramètres Discord et de changer votre mot de passe.
Pour changer le token d’un bot, il faut se rendre sur le Portail des Développeurs, sur votre application et réinitialiser le token directement.

À noter que depuis ces dernières années, Discord est en collaboration avec la plateforme de développement GitHub. Leur collaboration leur permet notamment de détecter les tokens mis en clair dans les codes sources et d’envoyer un message privé aux développeurs qui ont fait l’erreur de publier le token de leur bot. Il est également automatiquement réinitialisé pour des raisons de sécurité.

## Sécuriser un token

Un token ne peut pas approprement être sécurisé, c'est la sécurité de la machine où celui-ci est échangé et stocké qui importe réellement.

Voici une liste non exaustive des choses à ne surtout pas faire :

Pour un compte utilisateur,
- Installer un logiciel malveillant, un “jeu” envoyé en messages privés, une pièce téléchargeable envoyée par un utilisateur.
- Utiliser des scripts pour modifier votre interface Discord ou carrément faire usage d’un client (logiciel) qui n’est pas officiel (BetterDiscord, des plugins, ou autre solutions alternatives) qui peuvent compromettre la sécurité de votre compte.

Pour les bots,
- Partager le token avec d’autres utilisateurs, 
- Utiliser des logiciels qui permettent de connecter celui-ci
- Héberger son bot sur des hébergeurs qui ne sont pas sécurisés, reconnus et qui ne protègent pas les données personnelles.
- Ne pas mettre clairement le token dans le code.
