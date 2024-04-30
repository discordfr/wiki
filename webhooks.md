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

## Le fonctionnement et l'utilité du Webhooks
Un Webhook est une intégration au sein d'un serveur, permettant à des services externes tels que GitHub d'interagir avec le serveur par le biais d'envois de messages automatisés. Ce mécanisme repose sur l'utilisation d'une URL spécifique à placer sur le service externe désirant interagir avec le serveur. L'utilité des Webhooks se révèle utile dans de nombreux scénarios, telles que l'annonce du début d'un stream par un streamer à sa communauté ou la notification des développeurs quant aux derniers ajouts effectués sur GitHub.

![image webhook github](https://i.dfr.gg/ORnH.png)

## Création et Utilisation des Webhooks
### Création
La création d'un Webhook demeure la même pour tout service interagissant avec le serveur. Après avoir accédé aux paramètres du serveur, l'utilisateur doit naviguer jusqu'à la catégorie `Applications`, puis se diriger vers `Intégrations`. Une fois sur cette page, l'option `Webhooks` est accessible, où la création d'un nouveau Webhook est introduite par le bouton bleu intitulé `Nouveau Webhook`. Une fois cette étape franchie, la personnalisation du Webhook s'effectue en lui attribuant un nom et en sélectionnant le salon destinataire des messages.

![image creation webhook](http://i.dfr.gg/7JKT.png)

### L'utilisation
Une fois le Webhook créé, son utilisation se résume pour l'utilisateur à copier l'URL associée et à se rendre sur le service externe désiré afin de configurer les données à envoyer (Cette configuration peut être différente en fonction du service qui interagit avec le serveur)

:::note 
Les webhooks peuvent être utilisés avec n'importe quel service externe, y compris ceux que vous pourriez créer vous-même, discord ne limite pas à certain services.
:::

## L'exemple de Discohook
[Discohook](https://discohook.org/) représente un service externe parmi de nombreux autres qui permettent l'envoi de messages via des webhooks. Il démontre parfaitement la flexibilité des webhooks, qui peuvent être adaptés en fonction des besoins des utilisateurs. Le service offert par Discohook est simple : il permet d'envoyer des messages via des webhooks, que ce soit sous forme d'embeds ou de texte.

![image discohook](http://i.dfr.gg/I05C.png)
