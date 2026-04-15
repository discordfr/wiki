---
title: Les logs de serveur
keywords:
  - discord
  - serveur
  - logs
  - log
  - configuration
  - tutoriel
description: Les logs de serveurs
contributors: [luke, karal, dreas, chaussette]
---

Les logs (ou "journaux") du serveur permettent aux utilisateurs disposant de la permission appropriée de consulter une grande partie des actions effectuées sur un serveur.

__À noter :__ les entrées des logs sont conservées pendant environ 45 jours.

__Permission requise :__ *Voir les journaux d’audit*

## Les actions consignées

Les logs enregistrent différentes actions :

> Actions associées au serveur
- Mises à jour du serveur (modification d’icône, de nom, etc.)

> Actions associées aux salons
- Création de salons
- Modification des salons et de leurs permissions (overwrites)
- Suppression de salons
- Création, modification et suppression de threads (publics ou privés)

> Actions associées aux rôles
- Création de rôles
- Modification des rôles et de leurs permissions
- Suppression de rôles

> Actions associées aux membres
- Modification des rôles d’un utilisateur (ajout/retrait)
- Modification du surnom
- Expulsion de membres
- Suppression de membres inactifs (prune)
- Bannissement de membres
- Débannissement de membres
- Timeout (mise en sourdine temporaire)
- Déplacement vocal de membres
- Déconnexion vocale de membres

> Actions associées aux messages
- Suppression de messages  
  __Attention :__ le contenu du message n’est pas conservé dans les logs
- Suppression en masse de messages
- Épinglage et désépinglage de messages
- Messages bloqués ou signalés par AutoMod (selon la configuration)

> Autres actions
- Ajout de bots
- Création, modification et suppression d’invitations
- Création, modification et suppression de webhooks
- Création, modification et suppression d’emojis
- Création, modification et suppression d’intégrations
- Mise à jour des permissions des commandes d’application
- Création, modification et suppression d’autocollants
- Création, modification et suppression d’événements
- Création, modification et suppression de conférences
- Création, modification et suppression de sons (Soundboard)
- Création, modification et suppression de règles AutoMod
- Timeout appliqué automatiquement par AutoMod
- Création, modification et suppression du processus d’accueil
- Création et mise à jour du guide du serveur / page d’accueil

## Les filtres

Pour une recherche plus précise, des filtres sont utilisables : 
1. Les filtres d'utilisateurs.

![Les filtres d'utilisateurs](https://i.dfr.gg/stb.png)

2. Les filtres d'actions.

![Les filtres d'action](https://i.dfr.gg/F0I.png)
