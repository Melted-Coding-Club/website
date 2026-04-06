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
    celsius = float(input("Celsius for day " + str(day + 1) + ": "))
    fahrenheit = celsius * 9 / 5 + 32
    print("Day", day + 1, ":", celsius, "C =", round(fahrenheit, 1), "F")
```
