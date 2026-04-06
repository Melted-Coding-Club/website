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
n = int(input("Starting n (positive): "))
steps = 0

while n != 1:
    if n % 2 == 0:
        n = n // 2
    else:
        n = 3 * n + 1
    steps += 1

print("Steps to reach 1:", steps)
```
