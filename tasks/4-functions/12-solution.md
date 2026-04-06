---
layout: default
title: "Unit 4 Task 12 - Solution"
permalink: /tasks/4-functions/12-solution/
---

# Solution - Task 12: Three addition questions

[← Back to task]({{ site.baseurl }}/tasks/4-functions/12/)

---

One possible program:

```python
import random


def ask_addition():
    a = random.randint(1, 12)
    b = random.randint(1, 12)
    ans = int(input(f"What is {a} + {b}? "))
    return ans == a + b


def main():
    score = 0
    for _ in range(3):
        if ask_addition():
            score += 1
    print("Score:", score, "/ 3")


main()
```
