---
layout: default
title: "Unit 2 Task 47 - Solution"
permalink: /tasks/2-47-solution/
---

# Solution - Task 47: Battery drain simulation

[← Back to task]({{ site.baseurl }}/tasks/2-47/)

---

One possible program:

```python
import random

battery = 100
hours = 0

while battery > 0:
    drain = random.randint(5, 15)
    battery -= drain
    hours += 1
    print("After hour", hours, "battery ~", max(battery, 0))

print("Battery dead after", hours, "hours.")
```
