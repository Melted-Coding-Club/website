---
layout: default
title: "Unit 2 Task 18 - Solution"
permalink: /tasks/2-control-flow/18-solution/
---

# Solution - Task 18: Charity jar total

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/18/)

---

One possible program:

```python
total = 0.0

while True:
    donation = float(input("Donation amount (0 to finish): "))
    if donation == 0:
        break
    total += donation

print("Total raised:", total)
```
