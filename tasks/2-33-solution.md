---
layout: default
title: "Unit 2 Task 33 - Solution"
permalink: /tasks/2-33-solution/
---

# Solution - Task 33: Dice doubles at the café

[← Back to task]({{ site.baseurl }}/tasks/2-33/)

---

One possible program:

```python
import random

rolls = 0

while True:
    d1 = random.randint(1, 6)
    d2 = random.randint(1, 6)
    rolls += 1
    print(d1, d2)
    if d1 == d2:
        break

print("Rolls until doubles:", rolls)
```
