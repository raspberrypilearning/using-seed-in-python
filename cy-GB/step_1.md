Wrth greu rhifau ar hap gyda Python, fe allwch chi ddefnyddio **dosbarthiad** i gynhyrchu'r rhifau. Os byddwch chi'n dechrau gyda'r un dosbarthiad ac yn gofyn am yr un dilyniant o rifau, fe allwch chi greu nodwedd ar hap y gellir ei hailadrodd. Fe allai hyn fod yn ddefnyddiol i nifer o wahanol bethau, gan gynnwys:

- lleoli gwrthrychau ar y sgrin. Os ydych chi'n [llunio awyr y nos](https://trinket.io/python/c67c589510?outputOnly=true&runOption=run){:target="_blank"}, dydych chi ddim eisiau gorfod pigo safle pob seren!
- fel twyll, er enghraifft wrth daflu'r dis yn y prosiect [Helo fyd](https://projects.raspberrypi.org/en/projects/hello-world)
- creu bydoedd (fel yn Minecraft), gan benderfynu ble mae adnoddau a chreaduriaid yn cael eu lleoli ar hap


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