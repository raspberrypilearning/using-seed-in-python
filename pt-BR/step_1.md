Ao criar números aleatórios com Python, você pode usar uma **seed** para gerar os números. Se você começar da mesma seed e pedir a mesma sequência de números, poderá criar uma pseudo aleatoriadades. Algo que parece aleatório, mas não é. Isso pode ser útil para muitas coisas diferentes, incluindo:

- para posicionar objetos na tela. Se você está [desenhando o céu noturno](https://trinket.io/python/c67c589510?outputOnly=true&runOption=run){:target="_blank"}, você não quer escolher para onde cada estrela vai!
- para uma trapaça, como com o lançamento de dados no projeto [Hello World](https://projects.raspberrypi.org/pt-BR/projects/hello-world)
- para criar mundos (como no Minecraft), decidindo onde os recursos e as criaturas são colocadas aleatoriamente


Aqui está um exemplo usando `seed` como trapaça:

```python

from random import randint, seed

def load_dice():
  # Configura uma seed para sempre escolher o mesmo número
  seed('dice')
  roll = randint(1,6)
  print('Você rola', rola)

```
Este código gera:

```
Você tirou o número 4
```

**Dica:** Seed pode ser um número ou uma sequência de texto. Isso significa que pode ser um emoji também!
