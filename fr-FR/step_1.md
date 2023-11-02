Lors de la création de nombres aléatoires avec Python, tu peux utiliser **seed** pour générer les nombres. Si tu pars du même seed et demandes la même séquence de nombres, tu peux créer un caractère aléatoire imprévisible. Cela peut être utile pour de nombreuses choses différentes, notamment :

- pour positionner des objets sur l'écran. If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


Voici un exemple utilisant `seed` comme un tricheur :

```python

from random import randint, seed

def de_charge():
  # Défini une seed pour choisir toujours le même numéro
  seed('de')
  roll = randint(1,6)
  print('Tu as obtenu', roule)

```
Ce code affiche :

```
Tu as obtenu 4
```

**Astuce :** La valeur de départ peut être un nombre ou une chaîne de texte. Cela signifie que cela peut aussi être un emoji !
