---
title: Les clés de sécurité et Passkeys
keywords:
  - discord
  - conenxion
  - sécuité
  - comptes
  - tutoriel
description: Les clés de sécurité et Passkeys sur Discord
contributors: [mapidae]
short_slug: Passkeys
---

Les clés de sécurité sont LA SOLUTION pour rester en sécurité. Également connues sous le nom de clés d'authentification, elles sont des dispositifs physiques ou numériques utilisés pour renforcer la sécurité des comptes en offrant LA MEILLEURE solution d'authentification forte et à deux facteurs.

:::caution
Les clés de sécurité et Pass Keys n’empêchent pas certaines méthodes visant à récupérer le [jeton d’authentification du compte (token)](/wiki/confiance-securite/token). Sur Discord par exemple, un logiciel malveillant sur votre appareil peut intercepter votre token et accéder à votre compte comme s’il s'agissait de vous, sans la nécessité d’avoir des informations de connexion (identifiant, [mot de passe](/wiki/compte-utilisateur/authentification/mots-de-passe), numéro de téléphone, [A2F](/wiki/compte-utilisateur/authentification/a2f), clés de sécurité).
:::

## Fonctionnement

Ces clés fonctionnent comme des jetons d'authentification chiffré (tokens), qui offrent un niveau de sécurité élevé tout en éliminant la nécessité de mémoriser des mots de passe. Elles peuvent être stockées de manière sécurisée dans des dispositifs physiques ou synchronisées entre différents appareils via des services cloud. Elles sont généralement utilisées avec d'autres facteurs d'authentification, tels que la biométrie ou la possession d'un appareil spécifiques.

## Types de Clés de Sécurité

Les clés de sécurité physiques se présentent sous forme de périphériques USB, de cartes à puce ou de jetons. Elles génèrent des codes ou effectuent des opérations cryptographiques pour valider l'authentification.
Les clés de sécurité virtuelles sont intégrées à des services comme Dashlane ou d’autres qui sont dédiés à la sécurité numérique. 

## Différences

Les clés de sécurité offrent une authentification robuste, difficile à compromettre car il n’est pas possible de les synchroniser sur un site de phishing par exemple. 
Elles fournissent une méthode d'authentification simple pour les utilisateurs, ne nécessitant qu'une interaction physique avec le périphérique ou l'application. 
Leur utilisation et accessibilité
De nombreux services en ligne prennent en charge l'utilisation des clés de sécurité pour l'authentification à deux facteurs (A2F). Néanmoins les solutions physiques ne sont pour le moment pas très accessibles, en raison du prix de celles-ci qui peut démotiver la plupart des intéressés même si elles restent rentables à long terme. Les solutions numériques semblent plus accessibles financièrement à court terme.

## Recommandations

L'utilisation des clés de sécurité est recommandée pour renforcer la sécurité des comptes, surtout pour ceux qui gèrent des informations sensibles ou des données confidentielles comme les sites bancaires, les sites sensibles, ou d’autres services (Paypal, OVH, Google etc). Il est conseillé de choisir des clés compatibles avec les protocoles d'authentification standards tels que FIDO2 ou U2F pour une meilleure compatibilité avec une variété de services en ligne.

:::note 
L’utilisation des Passkeys avec des logiciels comme Dashlane ou autre peut permettre de savoir si le site est frauduleux. (Dashlane ne proposera pas la passkey "discord" si le site est "disc**a**rd")
:::

![Clés physiques VS Clés numériques](https://i.dfr.gg/3mgT.png)

