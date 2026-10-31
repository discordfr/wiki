---
title: Contribuer au wiki de Discord FR
description: Contribuer est la meilleure des actions à faire pour le wiki de Discord FR, apprenez comment nous aider sur cette page. :)
sidebar_label: Contribuer
short_slug: Contribuer
---

Sur cette page, vous apprendrez pas à pas à **créer une page** et **en modifier** pour devenir un vrai contributeur de ce wiki.
Elle vous expliquera les **bases et quelques conseils** utiles pour bien débuter.

## Différents moyens de nous aider

Pour contribuer à la rédaction d'un article du wiki, deux solutions s'offrent à vous :

* Envoyer le texte et images dans le salon `articles-wiki` de notre [serveur Discord des contributions](https://discord.com/invite/fkkCXsBrmE) ;
* Proposer vos changements directement depuis Github.

:::note
Le reste de la page correspond à la méthode avec Github.
Les [avantages et récompenses](#avantages-et-récompenses) sont communs à toutes les méthodes.
:::

## Initialisation

Si vous choisissez d'utiliser Github, il faut [se munir d'un compte](https://github.com/login).

Sur le [_repository_ du projet](https://github.com/discordfr/wiki) (dépôt), il faut [créer un _fork_](https://github.com/discordfr/wiki/fork) (copie).
C'est sur le fork que toutes les modifications et ajouts se font.

## Sélectionner le fichier

Les dossiers et fichiers portent les mêmes noms que le chemin dans l'URL.
Par exemple, [`https://dfr.gg/wiki/contenu-payant/abonnements-nitro`](/wiki/contenu-payant/abonnements-nitro) est présent dans le [dossier `contenu-payant`](https://github.com/discordfr/wiki/tree/master/contenu-payant), sous le nom [`abonnements-nitro.md`](https://github.com/discordfr/wiki/blob/master/contenu-payant/abonnements-nitro.md).

## Modifier un article

:::tip
Voir la section correspondante pour [en créer un nouveau](#créer-un-article).
:::

Sur la vue du contenu du fichier, en haut à droite, apparaît une icône stylo « 🖊️ ».
Le cliquer permet de débuter la modification du document.

![Bouton de modification](https://i.dfr.gg/CQgk.png)

:::note
Nous avons des [règles et habitudes de rédaction](#conventions-de-rédaction) qui sont à suivre.
:::

## Créer un article

:::tip
Voir la section correspondante pour [en modifier un existant](#modifier-un-article).
:::

Dans la vue du dossier parent, en haut à droite, apparaît un bouton « `Add file` ».
Le cliquer permet de débuter la création du document.

![Bouton de création de fichier](https://i.dfr.gg/41rD.png)

:::note
Nous avons des [règles et habitudes de rédaction](#conventions-de-rédaction) qui sont à suivre.
La création d'article doit être validée en amont avec les autres contributeurs sur [le serveur Discord des contributions](https://discord.com/invite/fkkCXsBrmE).
:::

## Finaliser les changements

Une fois le changement fait, il faut cliquer sur le bouton « `Commit changes…` ».
Sur le menu apparaissant alors, remplissez les différents encadrés puis cliquez sur « `Propose changes` ».

![Commentaires de modification](https://i.dfr.gg/3mzt.png)

## Proposer les changements

Une fois le _commit_ réalisé, la [création d'une _Pull Request_](https://github.com/discordfr/wiki/compare) (demande de changement) vous est suggéré.

Tout en bas de la page correspondante, toutes vos suppressions et ajouts sont listés.
C'est la dernière fois avant proposition que vous verrez votre texte ! Relisez-le une dernière fois.

![Liste des changements](https://i.dfr.gg/IXtf.png)

Si les changements ne vont pas, un lien vers votre _branch_ (branche) est disponible.
Vous pouvez y continuer vos changements.

![Lien vers la branche contenant les changements](https://i.dfr.gg/TKWE.png)

Sinon, renseignez les différents éléments demandés puis cliquez sur le bouton « `Create pull request` ».

:::note
Vous devez laisser la case « `Allow edits by maintainers` » cochée.
Cela permet à l'équipe de vous corriger, et continuer le suivi de la proposition quand vous n'êtes pas du tout disponible ou que vous ne souhaitez pas continuer.
:::

![Création d'une Pull Request](https://i.dfr.gg/gsYF.png)

## Vérification par l'équipe

L'équipe de _review_ de DFR ainsi que des contributeurs chevronnés examineront vos changements.

Si vous ne souhaitez pas vous occuper de l'application des demandes de modification, faites-le nous avoir !
De même si vous n'êtes que peu disponible ou si vous ne regardez que Discord et pas Github.
Nous vous remercions déjà grandement d'initier une amélioration du wiki.

L'écrasante majorité des changements ne sont pas parfaits dès la première fois – c'est normal.
Il faut alors appliquer les demandes de modification de l'équipe.

## Conventions de rédaction

Les fichiers utilisent le [format Markdown](https://markdownguide.org/cheat-sheet/) (fichiers `.md`).
Si des éléments supplémentaires sont utiles, des fichiers enrichis peuvent exister (`.mdx`), mais nous n'allons pas parler plus en détail de ceux-là – une connaissance légère en JavaScript étant requise.

### Front matter

C'est le bloc à mettre avant tout le contenu de la page (tirets autour compris) :

```yaml
---
title: Titre de l'article
keywords:
  - des
  - mots
  - clés
description: Une courte description du contenu de l'article.
contributors: [identifiants, venant, de, team.yml]
short_slug: false
---
```

Le contributeur qui se renseigne dans `contributors` doit aussi être ajouté dans [`team.yml`](https://github.com/discordfr/wiki/blob/master/team.yml).

### Format Markdown

| Syntaxe | Résultat |
| ------- | -------- |
| ## Titre 2 | <h2>Titre 2</h2> |
| ### Titre 3 | <h3>Titre 3</h3> |
| #### Titre 4 | <h4>Titre 4</h4> |
| ##### Titre 5 | <h5>Titre 5</h5> |
| ###### Titre 6 | <h6>Titre 6</h6> |
| \*\*Gras\*\* | **Gras** |
| \_Italique\_ | _Italique_ |
| \*\*\_Les deux cap'tain\_\*\* | **_Les deux cap'tain_** |
| > Citation | <blockquote><p><em>Citation</em></p></blockquote> |
| \* Liste à point | <ul><li>Liste à point</li></ul> |
| 1. Liste ordonnée | <ol><li>Liste ordonnée</li></ol> |
| \`code\` | `code` |
| --- | <hr /> |
| \[Lien externe\]\(https://dfr.gg/) | [Lien externe](https://dfr.gg/) |
| \[Lien interne\]\(/wiki/contribuer) | [Lien interne](/wiki/contribuer) |
| \!\[Image\]\(https://i.dfr.gg/JTH.png) | ![Image](https://i.dfr.gg/JTH.png) |

Chaque type d'élément markdown doit être séparés d'une ligne vide les uns des autres.

Un retour à la ligne doit être présent à la fin d'une phrase.
Tant qu'aucune ligne vide n'est écrite, le retour à la ligne continue le paragraphe avec un espace.

> Par exemple :

```md
La **roue** de mon _hamster quantique_ est sur ma table.
Mais, en fait, je n'ai ni hamster ni roue !

Par contre j'ai un géranium : juste [ici](https://i.dfr.gg/geranium.webm).
```

> Donne :

La **roue** mon _hamster quantique_ est sur ma table.
Mais, en fait, je n'ai ni hamster ni roue !

Par contre j'ai un géranium : juste [ici](https://i.dfr.gg/geranium.webm).

### Spécificités de Docusaurus

Le wiki fonctionne sur la base de [Docusaurus](https://docusaurus.io/docs/markdown-features).

#### Admonitions

Il en existe différents types :

* `note`, pour les remarques ;
* `tip`, pour les astuces (devrait être rare, un wiki n'est pas un guide) ;
* `info`, pour des informations annexes ;
* `warning`, pour mettre en avant une information importante ;
* `danger`, pour avertir le lecteur.

> Par exemple :

```md
:::tip
Vous pouvez utiliser les admonitions :]
:::
```

> Donne :

:::tip
Vous pouvez utiliser les admonitions :]
:::

## Avantages et récompenses

Après contribution, vous pourrez [obtenir des rôles](https://dfr.gd/avantages) sur [notre serveur Discord communautaire](https://discord.com/invite/fr).
Les **points méta** sont attribués à l'appréciation de l'équipe, selon la qualité de vos contributions.

Des accès supplémentaires sur [le serveur Discord des contributions](https://discord.com/invite/fkkCXsBrmE), tel que l'accès de salons réservé aux contributeurs, sont aussi donnés.
