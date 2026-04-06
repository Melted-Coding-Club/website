---
layout: default
title: "Unit 2 Task 45 - Solution"
permalink: /tasks/2-45-solution/
---

# Solution - Task 45: Sum of squares pyramid

[← Back to task]({{ site.baseurl }}/tasks/2-45/)

---

One possible program:

```python
n = int(input("n: "))
total = 0

for k in range(1, n + 1):
    total += k * k

print("Sum of squares:", total)
```
