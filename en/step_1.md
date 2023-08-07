When creating random numbers with Python, you can use a **seed** to generate the numbers. If you start from the same seed, and ask for the same sequence of numbers, then you can create repeatable randomness. This can be useful for many different things including:

- for positioning objects on the screen. If you're drawing the night sky, you don't want to pick where every star goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>
  
- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


Here is an example using `seed` as a cheat:

```python

from random import randint, seed

def loaded_dice():
  # Set a seed to always choose the same number
  seed('dice')
  roll = randint(1,6)
  print('You rolled', roll)

```
This code outputs:

```
You rolled 4
```

**Tip:** Seed can be a number, or a string of text. That means it can be an emoji too!
