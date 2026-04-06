---
layout: default
title: "Unit 2 Task 17 - Solution"
permalink: /tasks/2-control-flow/17-solution/
---

# Solution - Task 17: Five-question mental maths quiz

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/17/)

---

One possible program:

```python
import random

score = 0

for question_number in range(5):
    first_number = random.randint(1, 10)
    second_number = random.randint(1, 10)
    user_answer = int(input(f"What is {first_number} + {second_number}? "))
    if user_answer == first_number + second_number:
        score += 1

print("You scored", score, "out of 5")
```
