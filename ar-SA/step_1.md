عند إنشاء أرقام عشوائية باستخدام لغة Python، يمكنك استخدام الايعاز **seed بذور** لتوليد الأرقام. إذا بدأت من نفس البذرة ، وطلبت نفس تسلسل الأرقام ، فيمكنك إنشاء عشوائية قابلة للتكرار. يمكن أن يكون هذا مفيدًا للعديد من الأشياء المختلفة بما في ذلك:

- لوضع الأشياء على الشاشة. إذا كنت [ ترسم سماء الليل ](https://trinket.io/python/c67c589510?outputOnly=true&runOption=run){:target="_blank"}، لا تريد أن تختار أين يذهب كل نجم!
- كغش، كما هو الحال مع رمي النرد في مشروع [مرحبا بالعالم ](https://projects.raspberrypi.org/en/projects/hello-world)
- لإنشاء عوالم (كما في Minecraft) ، وتحديد مكان وضع المصادر والمخلوقات بشكل عشوائي


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