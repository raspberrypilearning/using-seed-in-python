Quando crei numeri casuali con Python, puoi impostare un seme con la funzione **seed** per generare i numeri. Se inizi dallo stesso seme e chiedi la stessa sequenza di numeri, puoi creare casualità ripetibile. Questo può essere utile per molte cose diverse, tra cui:

- per posizionare gli oggetti sullo schermo. Se stai disegnando un campo di asteroidi, non vuoi sicuramente decidere dove posizionare ogni singola roccia!

<iframe src="https://editor.raspberrypi.org/it-IT/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- come trucchetto, come abbiamo per il lancio dei dadi nel progetto [Hello World](https://projects.raspberrypi.org/it-IT/projects/hello-world)
- creare mondi (come in Minecraft), decidendo dove posizionare casualmente risorse e creature


Ecco un esempio che utilizza `seed` come trucco:

```python

from random import randint, seed

def lancia_dado():
  # Imposta un seed per scegliere sempre lo stesso numero
  seed('dadi')
  lancio = randint(1,6)
  print('Hai ottenuto', lancio)

```
Questo codice restituisce:

```
Hai ottenuto 4
```

**Suggerimento:** Il seme può essere un numero o una stringa di testo. Ciò significa che può essere anche un emoji!
