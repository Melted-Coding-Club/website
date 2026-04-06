---
layout: default
title: "Unit 2 Task 21 - Solution"
permalink: /tasks/2-21-solution/
---

# Solution - Task 21: Weekly step average

[← Back to task]({{ site.baseurl }}/tasks/2-21/)

---

One possible program:

```python
total = 0

for day in range(7):
    steps = int(input("Steps for day " + str(day + 1) + ": "))
    total += steps

average = total / 7
print("Average steps per day:", average)
```
