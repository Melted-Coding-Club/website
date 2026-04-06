---
layout: default
title: "Unit 2 Task 33 - Solution"
permalink: /tasks/2-control-flow/33-solution/
---

# Solution - Task 33: Dice doubles at the café

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/33/)

---

One possible program:

```python
import random

rolls = 0

while True:
    first_die = random.randint(1, 6)
    second_die = random.randint(1, 6)
    rolls += 1
    print(first_die, second_die)
    if first_die == second_die:
        break

print("Rolls until doubles:", rolls)
```
