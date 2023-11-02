Podczas tworzenia liczb losowych w Pythonie możesz użyć metody **seed** do wygenerowania liczb. Jeśli wykorzystasz ten sam seed i poprosisz o taką samą sekwencję liczb, możesz stworzyć powtarzalną losowość. To może być przydatne do wielu różnych rzeczy, w tym:

- do pozycjonowania obiektów na ekranie. If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


Oto przykład użycia `seed` jako oszustwo:

```python

from random import randint, seed

def obiążony_rzut():
  # Ustaw seed tak, aby zawsze wybierał tą samą liczbę
  seed('kość')
  rzut = randint(1,6)
  print('Wyrzuciłeś ', rzut)

```
Ten kod wyświetla:

```
Wyrzuciłeś 4
```

**Wskazówka:** Seed może być liczbą lub ciągiem tekstu. Oznacza to, że może to być również emoji!
