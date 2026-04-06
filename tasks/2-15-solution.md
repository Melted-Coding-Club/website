---
layout: default
title: "Unit 2 Task 15 - Solution"
permalink: /tasks/2-15-solution/
---

# Solution - Task 15: Higher–lower guessing game

[← Back to task]({{ site.baseurl }}/tasks/2-15/)

---

One possible program:

```python
import random

secret = random.randint(1, 100)
print("I'm thinking of a number from 1 to 100.")

while True:
    guess = int(input("Your guess: "))
    if guess < secret:
        print("Too low!")
    elif guess > secret:
        print("Too high!")
    else:
        print("Correct! Well done.")
        break
```
