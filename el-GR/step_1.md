Όταν δημιουργείς τυχαίους αριθμούς με την Python, μπορείς να χρησιμοποιήσεις τη συνάρτηση </strong>seed (σπόρος) **για να δημιουργήσεις τους αριθμούς. Εάν ξεκινήσεις από τον ίδιο σπόρο και ζητήσεις την ίδια ακολουθία αριθμών, τότε μπορείς να δημιουργήσεις επαναλαμβανόμενη τυχαιότητα. Αυτό μπορεί να είναι χρήσιμο για πολλά διαφορετικά πράγματα, όπως:</p>

- για την τοποθέτηση αντικειμένων στην οθόνη. If you're drawing an asteroid field, you don't want to pick where each rock goes!

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/dodge-asteroids-example" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
</iframe>

- as a cheat, like with the dice roll in the [Hello World](https://projects.raspberrypi.org/en/projects/hello-world) project
- to create worlds (like in Minecraft), deciding where resources and creatures are randomly placed


Ακολουθεί ένα παράδειγμα που χρησιμοποιεί τη συνάρτηση `seed` με εξαπάτηση:

```python

from random import randint, seed

def loaded_dice():
  # Ορισμός του σπόρου (seed) έτσι ώστε να επιλέγεται ο ίδιος αριθμός
  seed('dice')
  roll = randint(1,6)
  print('Εφερες', roll)

```
Αυτός ο κώδικας βγάζει:

```
Έφερες 4
```

**Συμβουλή:** Ο σπόρος μπορεί να είναι ένας αριθμός ή μια συμβολοσειρά κειμένου. Αυτό σημαίνει ότι μπορεί να είναι ακόμη και emoji!
