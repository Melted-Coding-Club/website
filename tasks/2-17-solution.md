---
layout: default
title: "Unit 2 Task 17 - Solution"
permalink: /tasks/2-17-solution/
---

# Solution - Task 17: Five-question mental maths quiz

[← Back to task]({{ site.baseurl }}/tasks/2-17/)

---

One possible program:

```python
import random

score = 0

for q in range(5):
    a = random.randint(1, 10)
    b = random.randint(1, 10)
    ans = int(input(f"What is {a} + {b}? "))
    if ans == a + b:
        score += 1

print("You scored", score, "out of 5")
```
