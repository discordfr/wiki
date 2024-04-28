---
title: L'authentification à deux facteurs (A2F)
keywords:
  - discord
  - a2f
  - authentification
  - tutoriel
  - compte
  - sécurité
description: Utilisation de l'authentification à deux facteurs sur Discord
contributors: [mapidae, ichii, volcanofr, xox]
short_slug: A2F
---

L'authentification à deux facteurs (A2F), également connue sous le nom de 2FA en anglais, est un mécanisme de sécurité renforcée qui vise à protéger l'accès aux comptes, comme Discord et d’autres services. En activant l'A2F, les utilisateurs ajoutent une couche de protection supplémentaire, nécessitant deux formes d'identification différentes pour accéder à leur compte. En plus du mot de passe habituel, l'utilisateur doit fournir une deuxième forme d'authentification, souvent quelque chose qu'il possède physiquement, comme un téléphone. Ce qui rend l’accès à un compte plus difficile pour des attaquants disposant du mot de passe.

:::note
La fonctionnalité de [QR Code](/wiki/compte-utilisateur/authentification/qr-code) passera toujours outre l'authentification à deux facteurs.
:::

Discord propose différents types d'A2F :

- Code renouvelé via une application : La deuxième couche est souvent un code généré régulièrement par une [application mobile comme Authy, Google Authenticator](/wiki/compte-utilisateur/authentification/mots-de-passe#bonnes-pratiques-gestion).
- Code par SMS ou e-mail : Ces méthodes offrent une sécurité en envoyant un code temporaire. Il est généralement composé de 4 à 6 chiffres, nécessaire pour permettre la connexion. Certains services exigent une vérification de connexion via un lien unique, ce qui permet d'approuver ou de refuser l'accès depuis une adresse IP ou un appareil spécifique.
- [Clé d'authentification physique ou numérique](/wiki/compte-utilisateur/authentification/cles-securite-passkeys) (passkeys / clés de sécurité) : Certains services peuvent utiliser en plus ou en remplacement des solutions habituelles, une clé physique ou une confirmation via une autre forme comme à partir d’une application sur smartphone.

Pour le cas de Discord, il s’agit des méthodes de code renouvelé via une application d’authentification, d’une validation par SMS ou d’une clé de sécurité. En revanche, ces méthodes doivent être activées manuellement par l'utilisateur.

## Choix de l’outil 

Lorsqu'il s'agit de choisir un bon outil d'authentification à deux facteurs, plusieurs options sont disponibles, chacune avec ses avantages spécifiques. 

De manière générale, les systèmes d’exploitation intègrent des solutions, comme du coté d’Apple qui propose sa solution intégrée “Apple Keychain” (Trousseau) qui  offre une sécurité robuste et est directement sauvegardé dans le cloud sur le compte Apple et synchronisé avec les appareils, ceci porte des avantages comme des inconvénients.

Authy et Google Authenticator par exemple proposent une solution plus souple en étant lié à un compte sécurisé, permettant une synchronisation aisée entre différents appareils, offrant ainsi une meilleure flexibilité.

Pour ceux qui utilisent des [gestionnaires de mots de passe](/wiki/compte-utilisateur/authentification/mots-de-passe#bonnes-pratiques-gestion) tels que Dashlane ou Bitwarden, l'A2F peut être gérée de manière centralisée, simplifiant ainsi la gestion des données de sécurité (selon le service et les options disponibles). Le choix entre ces outils dépendra des préférences individuelles en matière de sécurité, de facilité d'utilisation et de besoins spécifiques.

## Activation de l'A2F sur Discord

1. Installation de l'application d'authentification : Avant d'activer l'A2F, il est nécessaire d’installer une application d'authentification sur l’appareil, telle qu'Authy ou Google Authenticator. Il est aussi possible d’utiliser une solution incluse dans un [gestionnaire de mot de passe](/wiki/compte-utilisateur/authentification/mots-de-passe#bonnes-pratiques-gestion).
2. Accéder aux paramètres utilisateur : Dans Discord, il faut se rendre dans l'onglet "Paramètres" dans la catégorie "Mon Compte”.
3. Activation de l'A2F : Cliquer sur le bouton "Activer l'authentification à deux facteurs" et suivre les instructions.
4. Scan du QR Code ou saisie manuelle : Utiliser l’application d'authentification pour scanner le QR Code fourni ou entrer manuellement le code fourni.
5. Validation : Après avoir effectué ces étapes, un code à six chiffres sera fourni. Pour terminer, saisir ce code dans le champ prévu et cliquer sur "Activer."

## Codes de Secours

Lors de l'activation de l'A2F, Discord générera des codes de secours. Ces codes sont essentiels en cas de perte de l'application d'authentification. Il faut constamment s’assurer de les sauvegarder dans un endroit sûr comme dans des notes hébergées dans le cloud, imprimées ou sur un [gestionnaire de mots de passe](/wiki/compte-utilisateur/authentification/mots-de-passe#bonnes-pratiques-gestion).

:::caution Attention
Il ne faut pas les partager avec d’autres personnes ! En cas de perte des codes de secours et de l'impossibilité d'accéder à l'application d'authentification, Discord ne générera pas à nouveau ces codes.
:::

## Application de l'A2F sur un Serveur Discord

Les administrateurs de serveurs Discord peuvent imposer l'A2F aux membres, restreignant ainsi les actions de gestion et de modération aux seuls utilisateurs ayant activé l'A2F.

1. Dans les paramètres du serveur, accéder à l'onglet "Setup de Sécurité” puis “Permissions”.
2. Activer l'option "Exiger l'authentification à deux facteurs".
3. Saisir le code d'authentification généré sur l’application d'authentification.

:::note
Cette restriction s'applique instantanément aux membres du serveur qui ont des permissions spécifiques, cela les empêche de faire des actions de modération ou de configuration si la sécurité n’est pas activée.
::::

:::caution Attention
L'A2F n'est pas infaillible en cas de fuite du token d'authentification ou d'interaction avec un QR code malveillant.
:::
