Ao criar números aleatórios com Python, você pode usar uma **seed** para gerar os números. Se você começar da mesma seed e pedir a mesma sequência de números, poderá criar uma pseudo aleatoriadades. Algo que parece aleatório, mas não é. Isso pode ser útil para muitas coisas diferentes, incluindo:

- para posicionar objetos na tela. If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


Aqui está um exemplo usando `seed` como trapaça:

```python

from random import randint, seed

def load_dice():
  # Configura uma seed para sempre escolher o mesmo número
  seed('dice')
  rola = randint(1,6)
  print('Você tirou o número', rola)

```
Este código gera:

```
Você tirou o número 4
```

**Dica:** Seed pode ser um número ou uma sequência de texto. Isso significa que pode ser um emoji também!
