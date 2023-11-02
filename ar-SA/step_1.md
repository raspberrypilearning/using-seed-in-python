عند إنشاء أرقام عشوائية باستخدام لغة Python، يمكنك استخدام الايعاز **seed بذور** لتوليد الأرقام. إذا بدأت من نفس البذرة ، وطلبت نفس تسلسل الأرقام ، فيمكنك إنشاء عشوائية قابلة للتكرار. يمكن أن يكون هذا مفيدًا للعديد من الأشياء المختلفة بما في ذلك:

- لوضع الأشياء على الشاشة. If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


فيما يلي مثال باستخدام ` seed ` كغش:

```python

from random import randint, seed

def loaded_dice():
  # Set a seed to always choose the same number
  seed('dice')
  roll = randint(1,6)
  print('You rolled', roll)

```
الناتج من هذه الشفرة البرمجية:

```
You rolled 4
```

**نصيحة:** يمكن أن تكون البذور رقمًا أو سلسلة نصية. هذا يعني أنه يمكن أن يكون إيموجي أيضًا!
