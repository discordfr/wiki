---
title: AutoMod
keywords:
  - discord
  - automod
description: AutoMod
contributors: [ether]
short_slug: false
---

AutoMod est une fonctionnalité de Discord pour les serveurs "de communauté" (= Où la fonctionnalité de communauté est activée dans les paramètres de serveur) sortie en 2022 qui permet aux utilisateurs ayant les permissions "Gérer le serveur" ou "Administrateur" de mettre en place des filtres de mots clés et de spam qui pourront ensuite déclencher des actions de modération comme le bloquage de ces messages avant qu'ils ne soient envoyés, rendre muet un utilisateur et l'enregistrement des messages bloqués sous forme d'alertes dans un salon spécifié lors de la configuration des filtres. L'AutoMod peut être configuré en allant dans les paramètres de serveur puis dans le menu "AutoMod".

Discord propose trois configurations pré-définies d'AutoMod comme bloquer des mots fréquemment signalés, les spam de mentions utilisateur et des mots dans les noms de profil des membres.

Vous avez deux moyens pour créer un filtre de mots clés : 

- Utiliser les "caractères génériques", vous avez trois options : 

    - Utiliser `*` **en préfixe**, au moins un mot du message doit commencer par un mot clé.

    - Utiliser `*` **en suffixe**, au moins un mot du message doit se terminer par un mot-clé.

    - Utiliser `*` **n'importe où**, le mot-clé peut apparaître dans n'importe quelle partie du message, au mileu de n'importe quel mot.

*Voici des examples tirées de la [FAQ officielle sur l'AutoMod](https://support.discord.com/hc/fr/articles/4421269296535-FAQ-sur-l-AutoMod) :*

`cat*` --> get a **cat**-sitter
`*cat` --> cool bob**cat**
`*ana*` --> b**ana**nas 

Il y a cependant un autre moyen plus puissant en utilisant le regex/expression régulière.
