Lors de la création de nombres aléatoires avec Python, tu peux utiliser **seed** pour générer les nombres. Si tu pars du même seed et demandes la même séquence de nombres, tu peux créer un caractère aléatoire imprévisible. Cela peut être utile pour de nombreuses choses différentes, notamment :

- pour positionner des objets sur l'écran. Si tu [dessines le ciel nocturne](https://trinket.io/python/c67c589510?outputOnly=true&runOption=run){:target="_blank"}, tu ne veux pas choisir où va chaque étoile !
- comme un tricheur, comme avec le lancer de dés dans le projet [Hello World](https://projects.raspberrypi.org/fr-FR/projects/hello-world)
- pour créer des mondes (comme dans Minecraft), en décidant où les ressources et les créatures sont placées au hasard


Voici un exemple utilisant `seed` comme un tricheur :

```python

from random import randint, seed

def loaded_dice():
  # Set a seed to always choose the same number
  seed('dice')
  roll = randint(1,6)
  print('You rolled', roll)

```
Ce code affiche :

```
Tu as obtenu 4
```

**Astuce :** La valeur de départ peut être un nombre ou une chaîne de texte. Cela signifie que cela peut aussi être un emoji !

