---
layout: default
title: "Unit 2 Task 1 - Solution"
permalink: /tasks/2-control-flow/1-solution/
---

# Solution - Task 1: Running total at the bake sale

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/1/)

---

One possible program:

```python
total = 0.0

while True:
    amount = float(input("Enter payment (0 to finish): "))
    if amount == 0:
        break
    total += amount

print("Sum is:", total)
```
