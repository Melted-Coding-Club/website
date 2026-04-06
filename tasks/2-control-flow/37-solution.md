---
layout: default
title: "Unit 2 Task 37 - Solution"
permalink: /tasks/2-control-flow/37-solution/
---

# Solution - Task 37: Guess the product

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/37/)

---

One possible program:

```python
import random

first_factor = random.randint(1, 10)
second_factor = random.randint(1, 10)
product = first_factor * second_factor

while True:
    user_guess = int(input("Guess the product (two secret numbers 1-10): "))
    if user_guess == product:
        print("Correct! It was", first_factor, "x", second_factor)
        break
    if user_guess < product:
        print("Too low")
    else:
        print("Too high")
```
