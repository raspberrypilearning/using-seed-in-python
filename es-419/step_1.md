Si quieres crear números aleatorios con Python, puedes usar la función **semillas** para generar los números. Si comienzas desde la misma y pides la misma secuencia de números, puedes crear una aleatoriedad repetible. Esto te puede ser útil para muchas cosas, incluyendo las siguientes:

- para posicionar objetos en la pantalla. If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


A continuación hay un ejemplo donde se usa `semillas` como atajo:

```python

from random import randint, seed

def dado_cargado():
  # Establece el valor para seed (semilla) de tal manera que dado_cargado siempre arroje el mismo número
  seed('dado')
  tirar_dado = randint(1,6)
  print('Sacaste un', tirar_dado)

```
Este código da como resultado:

```
Sacaste un 4
```

**Consejo:** La semilla puede ser un número o una cadena de texto. ¡Eso significa que también puede ser un emoticón!
