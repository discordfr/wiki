---
title: Réduction de bruit, Krisp
keywords:
  - krisp
  - reduction de bruit
  - vocal
description: La réduction des bruits de fond en vocal, avec l'utilisation de Krisp
contributors: [antoww, volcanofr]
short_slug: krisp
---

Discord possède une fonctionnalité de **filtrage du bruit**.
Elle permet de réduire, pour les autres utilisateurs de la même session vocale, les bruits de fonds de l'utilisateur.
En éliminant les sons parasites tels que les bruits de clavier, les ventilateurs ou les voix éloignées, la qualité audio de l'utilisateur est améliorée.

## Paramétrage du profil d'entrée audio

Dans les **paramètres utilisateur**, menu "Voix & Vidéo" dans la section "Paramètres de l'appli", se trouve les paramètres de **profil d'entrée audio**.

Une sélection de 3 choix s'offrent alors à l'utilisateur :

- **Isolement de la voix**, applique la configuration optimale afin d'uniquement laisser la voix transparaître.
  Ce profil permet de configurer les paramètres suivant :
  - [Appuyer pour parler](#appuyer-pour-parler)
- **Studio**, qui ne définit aucun filtre et laisse tous les bruits passer.
  Ce profil ne donne pas accès à de configuration supplémentaire.
- **Personnalisés**, permettant un maximum de personnalisation.
  Ce profil permet de configurer les paramètres suivant :
  - [Ajuster automatiquement la sensibilité de la détection de la voix](#sensibilité-détection-voix)
  - [Suppression du bruit](#suppression-du-bruit)
  - [Annulation d'écho](#annulation-décho)
  - [Appuyer pour parler](#appuyer-pour-parler)

Quelque choix le profil sélectionné par l'utilisateur, les [paramètres vocaux avancés](#paramètres-vocaux-avancés) font partie de la configuration.

### Ajuster automatiquement la sensibilité de la détection de la voix {#sensibilité-détection-voix}

Sélection manuelle ou détection automatique de la sensibilité, bascule entre l'émission ou non de l'entrée audio.

### Suppression du bruit

Sélection de l'algorithme de suppression du bruit, parmis les choix suivants :

- Krisp, l'algorithme fait par [Krisp](https://krisp.ai/)
- Standard
- Aucun, désactive la suppression de bruit par défaut

### Annulation d'écho

Annule la révebération des sons de l'entrée audio.

### Appuyer pour parler

Définis comme pré-requis de l'émission de la voix l'appui sur des touches configurables.

### Paramètres vocaux avancés

#### Contrôle automatique de gain

Ajuste automatiquement le volume du microphone pour qu'il reste clair et constant.

#### Détection de la voix avancée

Règle un potentiel manque de détection automatique de la voix si désactivé.

#### Contournement du traitement des entrées audio du système

Désactive le traitement audio du système afin de ne pas interférer avec le traitement appliqué par Discord.

#### Avertissement d'audio non détecté

Affiche une fenêtre d'avertissement lorsque Discord ne détecte pas de son venant de l'entrée audio de l'utilisateur.

#### Avertissement de changement de salon vocal

Affiche une fenêtre de confirmation lorsque l'utilisateur souhaite passer d'une session vocale à une autre.

#### Atténuation globale

Diminue le volume des autres applications lorsqu'un son est émis de l'utilisateur ou reçus de la session.

#### Qualité de service

Informe le router de l'utilisateur que les paquets transmis par Discord sont de haute priorité.
Certains routers et fournisseurs de services internet peuvent agir de façon inhabituelle lorsque cette fonction est activée.

## Utilisation du filtrage audio

La réduction de bruit est **activée automatiquement** selon le profil d'entrée audio pour chaque utilisateur.

En cliquant sur l'icône de réduction de bruit, située dans la barre d'outils de l'appel, il est aussi possible de désactiver la suppression du bruit durant la session.

![Barre d'outils de l'appel](https://github.com/user-attachments/assets/57df0a36-7319-4508-b75e-7618cc1c238f)

## Fonctionnement de Krisp

Krisp utilise des algorithmes avancés de traitement du signal afin d'identifier et supprimer les bruits de fond tout en préservant la clarté de la voix.
Il fonctionne en temps réel, ce qui signifie que les utilisateurs peuvent bénéficier d'une réduction de bruit instantanée pendant leurs appels vocaux.
