---
layout: default
title: "Unit 2 Task 27 - Solution"
permalink: /tasks/2-27-solution/
---

# Solution - Task 27: US road trip temperatures

[← Back to task]({{ site.baseurl }}/tasks/2-27/)

---

One possible program:

```python
for day in range(7):
    c = float(input("Celsius for day " + str(day + 1) + ": "))
    f = c * 9 / 5 + 32
    print("Day", day + 1, ":", c, "C =", round(f, 1), "F")
```
