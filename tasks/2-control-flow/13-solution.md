---
layout: default
title: "Unit 2 Task 13 - Solution"
permalink: /tasks/2-control-flow/13-solution/
---

# Solution - Task 13: Waiting for a lucky 7

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/13/)

---

One possible program:

```python
import random

count = 0

while True:
    roll = random.randint(1, 10)
    count += 1
    print(roll)
    if roll == 7:
        break

print("It took", count, "attempts")
```
