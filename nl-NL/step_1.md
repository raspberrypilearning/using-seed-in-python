Wanneer je willekeurige getallen maakt met Python, kun je een **seed** gebruiken om de getallen te genereren. Als je vanuit dezelfde seed start en om dezelfde reeks getallen vraagt, kun je herhaalbare willekeur creëren. Dit kan voor veel verschillende dingen handig zijn, waaronder:

- voor het positioneren van objecten op het scherm. Bij het [tekenen van de nachtelijke hemel](https://trinket.io/python/c67c589510?outputOnly=true&runOption=run){:target="_blank"}, wil je niet steeds kiezen waar elke ster gaat!
- als een cheat, zoals bij de dobbelsteenworp in het [Hallo Wereld](https://projects.raspberrypi.org/en/projects/hello-world) project
- om werelden te creëren (zoals in Minecraft), en te beslissen waar middelen en wezens willekeurig worden geplaatst


Hier is een voorbeeld waarin `seed` als cheat wordt gebruikt:

```python

from random import randint, seed

def loaded_dice():
  # Set a seed to always choose the same number
  seed('dice')
  roll = randint(1,6)
  print('You rolled', roll)

```
Deze code geeft het volgende weer:

```
Je gooide 4
```

**Tip:** Seed kan een getal of een tekstreeks zijn. Dat betekent dat het ook een emoji kan zijn!