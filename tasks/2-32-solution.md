---
layout: default
title: "Unit 2 Task 32 - Solution"
permalink: /tasks/2-32-solution/
---

# Solution - Task 32: Collatz hailstone length

[← Back to task]({{ site.baseurl }}/tasks/2-32/)

---

One possible program:

```python
current_value = int(input("Starting n (positive): "))
steps = 0

while current_value != 1:
    if current_value % 2 == 0:
        current_value = current_value // 2
    else:
        current_value = 3 * current_value + 1
    steps += 1

print("Steps to reach 1:", steps)
```
