Pythonで乱数を作成する場合、乱数を生成する **seed** （シード）を使うことができます。 同じシードから始めて、同じ数字の並びを要求すると、再現性のあるランダム性を作ることができます。 これは、次のようなさまざまな用途に役立ちます。

- 画面上にオブジェクトを配置するため。 If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


チートとして `seed` を使用する例を次に示します。

```python

from random import randint, seed

def loaded_dice():
  # Set a seed to always choose the same number
  seed('dice')
  roll = randint(1,6)
  print('You rolled', roll)

```
このコードは以下を出力します。

```
さいころの目は4でした
```

**ヒント：** シードは、数値またはテキストの文字列にすることができます。 つまり、絵文字も使えるということです。
