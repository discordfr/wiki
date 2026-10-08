---
title: Les Webhooks sur Discord
keywords:
  - discord
  - webhooks
  - integrations
  - tutoriel
description: Un moyen simple et rapide pour envoyer des messages automatiques.
contributors: [antoine]
---

Un Webhook est une intégration au sein d'un serveur, permettant à des outils externes d'envoyer des messages sur un serveur. Le webhooks fonctionne grace à une URL à placer sur l'outil externe.

:::danger
Les webhooks peuvent représenter un danger. En cas de divulgation d'un lien de webhook, celui-ci peut devenir une porte d'entrée pour des attaques de serveur. Étant en mesure d'envoyer des messages vers un serveur, les webhooks peuvent être exploités afin d'effectuer des actions telles que qu'un envoi massif de mention, telles que l'utilisation de "@everyone".
:::

## Création
La création d'un Webhook demeure la même pour tout les outils. Après avoir accédé aux paramètres du serveur, l'utilisateur doit naviguer jusqu'à la catégorie `Applications`, puis se diriger vers `Intégrations`. Une fois sur cette page, l'option `Webhooks` est accessible, où la création d'un nouveau Webhook est introduite par le bouton bleu intitulé `Nouveau Webhook`. Une fois cette étape franchie, la personnalisation du Webhook s'effectue en lui attribuant un nom et en sélectionnant le salon destinataire des messages.

![image creation webhook](http://i.dfr.gg/7JKT.png)

## Utilisation
Une fois le Webhook créé, son utilisation se résume à copier l'URL associée et à se rendre sur l'outil externe désiré afin de le configurer (Cette configuration peut être différente en fonction du service qui interagit avec le serveur)

:::note 
Le webhook peut être utilisé avec n'importe quel service externe, y compris ceux que vous pourriez créer vous-même, discord ne limite pas à certain services.
:::

Le type de message que le webhooks envoie peut varier en fonction de ce qui est utilisé. Les messages peuvent être automatique et même manuel.

[Discohook](https://discohook.org/) est un outil externe parmi de nombreux autres qui permettent l'envoi de messages par la voie des webhooks mais de façon manuelle.

![image discohook](http://i.dfr.gg/I05C.png)