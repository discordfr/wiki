---
title: Ecriture Markdown
keywords:
  - discord
  - markdown
  - écriture
  - ecriture
  - tutoriel
description: Discord utilise le langage markdown pour permettre aux utilisateurs de mettre en forme leurs messages. Sa syntaxe simple lui permet d'éditer simplement et rapidement un message.
contributors: [xox, dragrame, freiik]
---

:::info Améliorations de la fonctionnalité Markdown
En juillet 2023, Discord a enrichi son support du format Markdown en introduisant des fonctionnalités supplémentaires telles que les entêtes, les liens masqués et les listes.
:::

## Syntaxe
La syntaxe Markdown se caractérise par le positionnement de caractères simples comme `*`, `_` ou encore `>`. Un exemple concret est le suivant :

```markdown
Le *pré* est rempli d'**animaux joyeux** chantant __gaiement__ ~~tant que le loup n'est pas là.~~
```
Affichera

<img alt="ExamplePhrase" src="https://i.discord.fr/HBj.png" class="docImage"/>

## Les entêtes
Pour créer un entête, il suffit d'inclure un nombre spécifique de caractères dièse (#). Il suffit d'utiliser `#` pour un gros entête, `##` pour un entête plus petit, ou `###` pour un entête encore plus petit en tant que premier(s) caractère(s) sur une nouvelle ligne pour créer un entête.

Par exemple, le message suivant :
```
# Gros entête

## Petit entête

### (encore) un petit entête
```
Donnera

<img alt="ExampleHeaders" src="https://i.volt.science/medias/Adam/l4tHP.png" class="docImage"/>

### Les liens masqués
Il est possible d'utiliser des liens masqués pour transformer un texte en un lien hypertexte cliquable ou activable. Pour ce faire, il suffit d'inclure le texte voulu entre crochets, suivi de l'URL entre parenthèses.

À titre d'exemple, le message suivant :
```
Voici un lien masqué pour voir le site internet [Discord.fr](https://discord.fr) !
```
Montrera

<img alt="ExampleMaskedLink" src="https://i.volt.science/medias/Adam/9567u.png" class="docImage"/>

### Les listes
Pour créer une liste, il suffit de commener chaque élément de la liste par un tiret (-) suivi d'un espace, ou par un astérisque suivi d'un espace.

Par exemple, la liste suivante :
```
- Pain
* Fromage
- Vin
```
Donnera

<img alt="ExampleList" src="https://i.volt.science/medias/Adam/i2DMF.png" class="docImage"/>

:::tip
Il est également possible d'ajouter de l'indentation aux éléments d'une liste en ajoutant des espaces avant le tiret ou l'astérisque.

![Liste indentée](https://i.volt.science/medias/Adam/aMx5w.png)
![Liste indentée](https://i.volt.science/medias/Adam/kHbSA.png)
:::

## Les blocs de citation
Discord permet également de [citer](https://discord.fr/wiki/interface/salon-textuel/citations) d'autres messages. Cette mise en forme est réalisable en mettant le signe `>` devant une nouvelle ligne. Ce qui donnera :

<img alt="ExampleQuote" src="https://i.discord.fr/EV1.png" class="docImage"/>

## Les blocs spoilers
Durant l'année 2019 Discord a ajouté les blocs de spoilers. Cette fonctionnalité fonctionne comme le reste de la mise en forme Markdown. Elle permet de cacher du texte à la première vue d'un utilisateur, et donc ainsi de ne pas dévoiler une chose importante sur un film par exemple à des utilisateurs ne voulant pas connaitre la fin en avance. Pour mettre des spoilers dans un message, il faut utiliser la commande implémentée dans Discord /spoiler (qui cachera la totalité du message) ou entourer la zone à cacher avec deux caractères `||`. Ce qui affichera :

<img alt="ExampleSpoilers" src="https://i.discord.fr/vmX.png" class="docImage"/>

## Les blocs de code
Il est aussi possible de formater du texte sous forme de code. Il suffit de mettre \`\`\` devant puis le langage (exemples : `js`, `java`, `css`, `html`) et de fermer le code de la même manière \`\`\`. 

![Code](https://i.discord.fr/N2S.png)

:::tip
Il est possible de mettre un message en couleur en utilisant ce même markdown. 

![Couleurs écrire](https://i.discord.fr/zJV.png)
![Couleurs écrire](https://i.discord.fr/Dow.png)
:::

## La mise en forme rapide
Pour faciliter l'utilisation de la mise en forme, Discord a également ajouté une fonctionalité de mise en forme rapide (Disponible uniquement sur l'application Windows, Linux, MacOS ainsi que l'application Web). Pour l'utiliser, il suffit de sélectionner avec la souris ou le clavier la zone à modifier et plusieurs boutons apparaîtront pour mettre en forme le texte:

<img alt="Selector" src="https://i.discord.fr/ejU.png" class="docImage"/>

## Les raccourcis claviers
Plusieurs raccourcis claviers sont disponible pour gagner du temps lors de la mise en forme. Pour les utiliser il suffit de sélectionner le texte à mettre forme et effectuer une combinaison de touche comme suit:

- <kbd>Ctrl</kbd> + <kbd>I</kbd>: *Italique*
- <kbd>Ctrl</kbd> + <kbd>B</kbd>: **Gras**
- <kbd>Ctrl</kbd> + <kbd>U</kbd>: <u>Souligné</u>

*Une liste plus complète de la syntaxe Markdown est disponible [ici](https://www.markdownguide.org/cheat-sheet/).*
