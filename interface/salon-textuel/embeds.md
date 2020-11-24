# Qu'est ce qu'un embed ?
Un embed est une forme de message differente de ceux que nous voyons habituellement 
<br>
<img src="https://zupimages.net/up/20/48/r53x.png">
<br>
Les embeds sont extrement personnalisables que ce soit la couleur la taille du texte les images intégrées et beaucoup plus 
# Comment les utiliser ?
Pour l'instant, les embeds ne sont utilisables que par les comptes bot
et ne sont pas disponibles pour les utilisateurs normals
# Comment utiliser les embeds en tant que developpeur de bot ? 
### En javascript 
En javascript, avec le module "discord.js" ( npm install --save discord.js ), Discord possede une classe "MessageEmbed" qui sert a créer des messages embed
Syntaxe : 
  - Faire un embed:
    - ```const embed = new Discord.MessageEmbed()```
            <br>
            ```.setTitle('Votre titre')```
            <br>
            ```.setDescription('votre description')```
            <br>
            ```.addField('titre du nouveau champ', 'contenu du nouveau champ')```
            <br>
            ```.setImage("lien direct vers votre image")```
            <br>
            ```.setThumbnail('lien de votre miniature')```
            <br>
            ```.setColor(<colorResolvable>)```
            <br>
            ```.setAuthor("Nom de l'autheur", "lien de l'icon de l'autheur")```
            <br>
            ```.attachFiles(<file>)```
  - Envoyer l'embed:
      - ```<TextChannel>.send(embed)```
Toutes les fonctions montrées sont OPTIONNELLES, ne pes spécifier d'image (```.setImage```) n'a aucun impacte etc.
