---
title: Les serveurs de Guildes
keywords:
  - discord
  - guildes discord
  - recrutement discord
  - tag de guilde
  - gestion de guilde
  - communauté gaming
description: Fonctionnement des Guildes sur Discord, une expérimentation permettant aux joueurs de créer des communautés exclusives avec un système de recrutement avancé, une gestion optimisée et une identité visuelle unique.
contributors: [derrios]
short_slug: false
---

Les **Guildes** sont une fonctionnalité de Discord visant à structurer les communautés de joueurs en proposant un format intermédiaire entre les **serveurs privés d'amis** et les **serveurs communautaires**. Leur particularité repose sur un **système de candidature** et un **tag personnalisé** attribué aux membres acceptés.

:::note
L'expérimentation des Guildes sur Discord est une fonctionnalité en cours de test et est susceptible de changer ou d'être retirée à l'avenir.
:::

## Caractéristiques principales
- **Limitation** : Une Guilde peut accueillir jusqu'à **200 membres maximum**.
- **Système de candidature** : Tout utilisateur doit **envoyer une candidature** pour rejoindre une Guilde. Les administrateurs et modérateurs possédant la permission d'expulsion (kick) peuvent **accepter, refuser ou discuter** avec le candidat dans un groupe privé sans avoir besoin de l’ajouter en ami.
- **Tag personnalisé** : Chaque Guilde dispose d'un **tag**, affiché sur le **profil public** des membres. Un utilisateur ne peut afficher qu'un seul tag à la fois s’il est dans plusieurs Guildes.

## Création et Gestion
### Activation et désactivation
L'activation de la fonctionnalité **n’impacte pas** la structure existante du serveur. Une fois transformé en Guilde, un serveur conserve ses canaux, rôles et permissions. En revanche, **la désactivation est définitive** et entraîne la suppression des candidatures en attente.

:::tip
Avant de désactiver une Guilde, il est recommandé de sauvegarder les candidatures en cours, car elles seront définitivement perdues.
:::

### Paramètres et Personnalisation
Les **paramètres des Guildes** sont accessibles dans **"Guild Settings"** sous l’onglet des paramètres du serveur. Les options de personnalisation comprennent :
- **Un tag** unique en quatre caractères.
- **Un icône** et **une bannière** associés à la Guilde.
- **Un tag** visible sur le profil des membres.

## Fonctionnalités et Limitations
### Fonctionnalités disponibles
- **Système de candidature intégré** (avec possibilité d’échanger avec le candidat avant validation).
- **Affichage du tag Guilde sur le profil** des membres.
- **Possibilité pour les administrateurs de modifier les paramètres** de la Guilde à tout moment.
- **Historique des candidatures** conservé pendant **180 jours**.

:::tip
Les candidatures refusées ou acceptées restent consultables pendant 180 jours, ce qui permet d'analyser le recrutement passé.
:::

### Limitations
- **Aucune option de modération spécifique** : Les Guildes n’intègrent pas d’outils avancés pour gérer les candidatures ou les comportements des membres.
- **Pas de journal d’activité** : Aucune trace des actions liées aux candidatures n'est enregistrée.
- **Pas d'intégration spécifique aux jeux** : Les Guildes ne bénéficient pas d’outils particuliers pour l’organisation d’activités en jeu.
- **Une seule Guilde affichable par utilisateur** : Un membre ne peut montrer qu’un seul tag, même s’il fait partie de plusieurs Guildes.

:::caution
Les Guildes ne disposent pas d’un système de logs des activités des membres. Il est recommandé d’utiliser des bots tiers pour pallier cette limitation.
:::

## Notes et astuces supplémentaires

- **Les tags disparaissent immédiatement** du profil des membres dès qu’ils quittent une Guilde.
- **Les candidatures ne peuvent pas être récupérées** après désactivation de la Guilde.
- **Les rôles et canaux sont préservés** lors de la conversion d’un serveur en Guilde.
