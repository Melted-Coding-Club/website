---
layout: default
title: "Unit 2 Task 50 - Solution"
permalink: /tasks/2-50-solution/
---

# Solution - Task 50: Delivery van route checker

[← Back to task]({{ site.baseurl }}/tasks/2-50/)

---

One possible program:

```python
capacity = float(input("Van capacity (kg): "))
load = 0.0

while True:
    package_weight = float(input("Next package kg (0 to finish): "))
    if package_weight == 0:
        break
    if load + package_weight > capacity:
        print("Overloaded - cannot load")
        break
    load += package_weight

print("Final load (kg):", load)
if load >= capacity:
    print("At or above capacity.")
else:
    print("Under capacity.")
```
