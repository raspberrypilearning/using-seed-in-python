Wrth greu rhifau ar hap gyda Python, fe allwch chi ddefnyddio **dosbarthiad** i gynhyrchu'r rhifau. Os byddwch chi'n dechrau gyda'r un dosbarthiad ac yn gofyn am yr un dilyniant o rifau, fe allwch chi greu nodwedd ar hap y gellir ei hailadrodd. Fe allai hyn fod yn ddefnyddiol i nifer o wahanol bethau, gan gynnwys:

- lleoli gwrthrychau ar y sgrin. If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


Dyma enghraifft yn defnyddio `dosbarthiad` fel twyll:

```python

from random import randint, seed

def loaded_dice():
  # Gosodwch ddosbarthiad i ddewis yr un rhif bob tro
  seed('dis')
  tafliad = randint(1,6)
  print('Rydych chi wedi taflu', tafliad)

```
Mae'r cod hwn yn allbynnu:

```
Rydych chi wedi taflu 4
```

**Cyngor:** Mae dosbarthiad yn gallu bod yn rhif neu'n llinyn testun. Mae hynny'n golygu ei fod yn gallu bod yn emoji hefyd!
