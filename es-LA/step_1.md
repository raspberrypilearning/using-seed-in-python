Si quieres crear números aleatorios con Python, puedes usar la función **seed** (semilla) para generar los números. Si comienzas desde la misma seed (semilla) y pides la misma secuencia de números, puedes crear una aleatoriedad repetible. Esto te puede ser útil para muchas cosas, incluyendo las siguientes:

- para posicionar objetos en la pantalla. Si estás trabajando en el proyecto [dibujando el cielo nocturno](https://trinket.io/python/c67c589510?outputOnly=true&runOption=run){:target="_blank"}, ¡no querrás elegir la posición para cada estrella!
- para usar como atajo, como cuando tires los dados en el proyecto [Hola Mundo](https://projects.raspberrypi.org/es-LA/projects/hello-world)
- para crear mundos (como en Minecraft), decidiendo aleatoriamente la ubicación de los recursos y las criaturas


A continuación hay un ejemplo donde se usa `seed` (semilla) como atajo:

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

**Sugerencia:** Seed (semilla) puede ser un número o una cadena de texto. ¡Eso significa que también puede ser un emoji!
