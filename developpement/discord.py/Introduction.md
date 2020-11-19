# Discord.py

## Introduction

### Pré requie :
Dans un premier temps pour pouvoir faire votre bot discord en python il va vous falloir vous munir de [l'IDLE python](https://www.python.org/downloads/) et de la librery discord.py (py -m pip install -U discord.py)
Une fois que vous aurez cela d'installer vous pourrez commencer à construire votre bot. Pour cela il va falloir importée les libreri et crée une varibale pour votre bot :

```python
import discord
from discord.ext import commands

bot = commands.Bot(command_prefix = "!", description = "description de mon super bot !")
```

### Premier Event et démarage du bot :
ensuite une fois cela fais vous allez devoir crée un event pour voir si le Bot et bien allumée :
```python
@bot.event
async def on_ready():
  print("Bot ON")
```

Et pour terminer vous allez devoir "run" le bot (l'allumer) :

```python
bot.run("TOKEN DU BOT")
```

Si vous ne savez pas où trouvé le Token de votre bot, vous allez vous rendre sur discord.dev puis crée une nouvelle application et crée un bot, puis clické sur "copier le Token".

![capture1](https://cdn.discordapp.com/attachments/650758414791606313/779079354592002108/Capture15.PNG)
![capture2](https://cdn.discordapp.com/attachments/650758414791606313/779079355758411796/Capture16.PNG)
![capture3](https://cdn.discordapp.com/attachments/650758414791606313/779079358098440193/Capture18.PNG)
![capture4](https://cdn.discordapp.com/attachments/650758414791606313/779079361206288414/Capture19.PNG)
