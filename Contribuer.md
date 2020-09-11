---
id: Contribuer
title: Contribuer au Wiki de DiscordFR
description: Contribuer est une chose importante pour le Wiki de DiscordFR, Apprenez comment nous aider sur cette page :)
image: https://i.discord.fr/9yU.png
---
# Contribuer au Wiki de DiscordFR
Dans cet article, vous apprendrez pas à pas à créer une page et à la modifier pour devenir un vrai contributeur de ce Wiki. Elle vous expliquera les bases et quelques conseils utiles pour bien débuter.

### Comment modifier une page du Wiki #

#### Sélection du Fichier
Rendez vous sur la page [GitHub du Wiki](https://github.com/discordfr/wiki) puis choissisez le fichier que vous souhaitez éditer dans la liste.

![Choisir un Fichier](https://i.discord.fr/X6T.png)
:::note Note
Les fichiers portent le nom du lien, par exemple Contribuer.md est le fichier correspondant au lien https://discord.fr/wiki/Contribuer.
:::

#### Débuter la modification
Cliquez sur le petit logo de crayon (Modifier), GitHub alors créra automatiquement une "Fork" dans votre profil, ce qui vous permettra de modifier le document.

![Modifier](https://i.discord.fr/TPF.png)

#### Valider la modification et la commenter
Après avoir fait vos modifications, Mettez un commentaire qui explique précisément vos modifications, vous devez ___indiquer vos sources___ si vous en avez. (Numéro 1)

Puis validez en appuyant sur le bouton "Propose changes" qui confirmera l'action. (Numéro 2)

![Commenter](https://i.discord.fr/KYW.png)
:::caution Attention !
Même si un membre de l'équipe passe derrière, relisez vous. Les modifications ayant un nombre trop important de fautes d'orthographes seront écartés.
:::

#### Vérification et mise en ligne
C'est la dernière fois que vous verrez votre texte ! Relisez le une dernière fois. (Numéro 1)

Une fois que vous êtes certain du contenu, appuyez sur "Create pull request". (Numéro 2)

![Pull Request Creation](https://i.discord.fr/5TM.png)

#### Création de la Pull Request
Ici vous pouvez pour la dernière fois modifier le titre et le commentaire d'ajout. Vérifiez si il est complet et ci possible sourcé (Un article du support anglophonne par exemple). (Numéro 1)

Ensuite pour terminer votre travail, appuyez sur "Create pull request". (Numéro 2)

:::caution Attention !
Vous devez laisser coché la case "Allow edits by maintainers" pour nous autoriser la correction de fautes ou tout simplement nous permettre j'ajouter les tags nécessaires pour que notre site web ultra méga high tech puisse fonctionner.
:::

![Pull Request Creation 2](https://i.discord.fr/Xf5.png)

#### Vérification par l'équipe
Si vous tombez sur la page suivante, vous n'avez plus rien à faire, le staff de DiscordFR et les contributeurs chevronnées examinerons votre modification.

![Finish](https://i.discord.fr/bib.png)
:::info Information
Il faudra à l'équipe moins d'une semaine pour examiner votre modification. Si cepandant vous constatez que cela prends plus de temps, vous pouvez directment nous contacter sur [Notre Discord](https://discord.gg/fr) en envoyant un Message Privé au bot Discord FR#9922.
:::

*********************

### Comment ajouter une page au Wiki #

#### Créer une page vide prête à remplir
Rendez vous sur la page [GitHub du Wiki](https://github.com/discordfr/wiki), ensuite choissisez "Add File" puis "Create new file"

![Add file button](https://i.discord.fr/wtU.png)

#### Ajouter le contenu de base
Comme pour la modification, entrez le contenu initiale de la page. (Numéro 1)

Une fois le contenu rempli, indiquez ce que cette page initiale contient, et ci-possible, ajoutez des sources. (Numéro 2)

:::danger Attention !!!
Pensez à nommer votre fichier en haut (wiki/nom). **Mettez impérativement .md à la fin du fichier, sans cela votre page ne fonctionnera pas et sera rejeté**
:::

Une fois tout correctement rempli, relisez vous attentivement, puis ensuite appuyez simplement sur "Propose new file". (Numéro 3)

:::caution Attention !
Même si un membre de l'équipe passe derrière, relisez vous. Les modifications ayant un nombre trop important de fautes d'orthographes seront écartés.
:::

![Initial Content](https://i.discord.fr/o3A.png)

#### Vérification et mise en ligne
Encore une fois c'est la dernière fois que vous verrez votre texte ! Relisez le une dernière fois. (Numéro 1)

Une fois que vous êtes certain du contenu, appuyez sur "Create pull request". (Numéro 2)

![Pull Request Creation addpage](https://i.discord.fr/Pwy.png)

#### Création de la Pull Request
Ici vous pouvez pour la dernière fois modifier le titre et le commentaire d'ajout. Vérifiez si il est complet et ci possible sourcé (Un article du support anglophonne par exemple). (Numéro 1)

Ensuite pour terminer votre travail, appuyez sur "Create pull request". (Numéro 2)

:::caution Attention !
Vous devez laisser coché la case "Allow edits by maintainers" pour nous autoriser la correction de fautes ou tout simplement nous permettre j'ajouter les tags nécessaires pour que notre site web ultra méga high tech puisse fonctionner.
:::

![Pull Request Creation addpage 2](https://i.discord.fr/3n6.png)

#### Vérification par l'équipe
Si vous tombez sur la page suivante, vous n'avez plus rien à faire, le staff de DiscordFR et les contributeurs chevronnées examinerons votre nouvelle page.

![Finish addpage](https://i.discord.fr/bib.png)
:::info Information
Il faudra à l'équipe moins de deux semaines pour examiner votre nouvelle page. Si cepandant vous constatez que cela prends plus de temps, vous pouvez directment nous contacter sur [Notre Discord](https://discord.gg/fr) en envoyant un Message Privé au bot Discord FR#9922.
:::

*********************

### Bonus pour les nerds #

#### Ajouter les balises Docusaurus dans la création de la page

Vous pouvez faciliter le travail de l'équipe en rajoutant les [Balises Docusaurus](https://v2.docusaurus.io/docs/markdown-features/#markdown-headers)

Vous pouvez ajouter les balises suivantes:
- title
- keywords
- description

Voila ce que devrait donner le début de votre document par exemple:

```yaml
---
title: Contribuer
keywords:
  - contribuer
  - discord
  - wiki
  - tutoriel
description: Contribuer est une chose importante pour le Wiki de DiscordFR, Apprenez comment nous aider sur cette page :)
---

```
:::tip Truc et Astuce
Vous pouvez regarder la construction des articles déja en ligne pour copier des éléments, comme ces boites d'information, ou vous pouvez aller sur le site de Docusaurus, Ces fameuses boites sont expliqués [dans cet extrait](https://v2.docusaurus.io/docs/markdown-features/#calloutsadmonitions)
:::

#### Liens pour les nerds

[Docusaurus V2 Markdown](https://v2.docusaurus.io/docs/markdown-features/) (Anglais)
