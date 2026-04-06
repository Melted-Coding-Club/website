---
layout: default
title: "Unit 3 Task 11 - Solution"
permalink: /tasks/3-data-structures/11-solution/
---

# Solution - Task 11: Cafe menu order total

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/11/)

---

One possible program:

```python
menu = {"coffee": 3.5, "muffin": 2.0, "juice": 4.0}
total = 0.0

while True:
    item = input("Order item (or 'done'): ").strip().lower()
    if item == "done":
        break
    if item in menu:
        total += menu[item]
    else:
        print("Not on menu")

print("Total: $", round(total, 2))
```
