---
layout: default
title: "Unit 2 Task 18 - Solution"
permalink: /tasks/2-18-solution/
---

# Solution - Task 18: Charity jar total

[← Back to task]({{ site.baseurl }}/tasks/2-18/)

---

One possible program:

```python
total = 0.0

while True:
    d = float(input("Donation amount (0 to finish): "))
    if d == 0:
        break
    total += d

print("Total raised:", total)
```
