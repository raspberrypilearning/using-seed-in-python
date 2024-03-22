Wanneer je willekeurige getallen maakt met Python, kun je een **seed** gebruiken om de getallen te genereren. Als je vanuit dezelfde seed start en om dezelfde reeks getallen vraagt, kun je herhaalbare willekeur creëren. Dit kan voor veel verschillende dingen handig zijn, waaronder:

- voor het positioneren van objecten op het scherm. Als je een asteroïdeveld tekent, wil je niet kiezen waar elke steen naartoe gaat!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- als cheat, zoals bij de dobbelsteenworp in het [Hallo Wereld](https://projects.raspberrypi.org/nl-NL/projects/hello-world) project
- om werelden te creëren (zoals in Minecraft), en te beslissen waar middelen en wezens willekeurig worden geplaatst


Hier is een voorbeeld waarin `seed` als cheat wordt gebruikt:

```python

from random import randint, seed

def nep_dobbelsteen():
  # Stel de seed zo in dat nep_dobbelsteen altijd hetzelfde getal gooit
  seed('dobbelsteen')
  worp = randint(1,6)
  print('Je gooide', worp)

```
Deze code geeft het volgende weer:

```
Je gooide 2
```

**Tip:** Seed kan een getal of een tekstreeks zijn. Dat betekent dat het ook een emoji kan zijn!

