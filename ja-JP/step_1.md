Pythonで乱数を作成する場合、乱数を生成する **seed** （シード）を使うことができます。 同じシードから始めて、同じ数字の並びを要求すると、再現性のあるランダム性を作ることができます。 これは、次のようなさまざまな用途に役立ちます。

- 画面上にオブジェクトを配置するため。 [夜空を描く](https://trinket.io/python/c67c589510?outputOnly=true&runOption=run){:target="_blank"}場合、星の一つ一つをどこに置くか決めたくはないでしょう!
- [ハローワールド](https://projects.raspberrypi.org/ja-JP/projects/hello-world) プロジェクトのサイコロ振りのようにチートとして
- （Minecraftのように）世界を作成し、リソースとクリーチャーをランダムに配置する場所を決めるため


チートとして `seed` を使用する例を次に示します。

```python

from random import randint, seed

def loaded_dice():
  # loaded_dice関数が一連の数字を出すようにシードを設定する
  seed('dice')
  roll = randint(1,6)
  print('サイコロの目はこれでした ', roll)

```
このコードは以下を出力します。

```
さいころの目は4でした
```

**ヒント：** シードは、数値またはテキストの文字列にすることができます。 つまり、絵文字も使えるということです。
