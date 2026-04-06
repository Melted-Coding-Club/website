---
layout: default
title: "Unit 2 Task 37 - Solution"
permalink: /tasks/2-37-solution/
---

# Solution - Task 37: Guess the product

[← Back to task]({{ site.baseurl }}/tasks/2-37/)

---

One possible program:

```python
import random

a = random.randint(1, 10)
b = random.randint(1, 10)
product = a * b

while True:
    g = int(input("Guess the product (two secret numbers 1-10): "))
    if g == product:
        print("Correct! It was", a, "x", b)
        break
    if g < product:
        print("Too low")
    else:
        print("Too high")
```
