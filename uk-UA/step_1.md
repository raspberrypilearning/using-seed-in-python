Створюючи випадкові числа у Python, ти можеш використати **seed**, щоб генерувати числа. Якщо ти використовуєш один і той же seed, і задаєш одну і ту ж послідовність чисел, то можеш створити повторювану випадковість. Це може бути корисно в багатьох випадках, наприклад:

- для розташування об'єктів на екрані. If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


Ось приклад використання `seed` як чит-коду:

```python

from random import randint, seed

def завантажені_кубики():
  # Встанови seed, щоб завжди використовувати це число
  seed('кубики')
  roll = randint(1,6)
  print('Тобі випало:', roll)

```
Цей код виведе:

```
Тобі випало: 4
```

**Порада:** Seed може бути як числом, так і текстом. Це означає, що він теж може бути емодзі!
