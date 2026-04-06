---
layout: default
title: "Unit 2 Task 20 - Solution"
permalink: /tasks/2-20-solution/
---

# Solution - Task 20: Factorial orderings

[← Back to task]({{ site.baseurl }}/tasks/2-20/)

---

One possible program:

```python
n = int(input("N: "))
result = 1

for i in range(1, n + 1):
    result *= i

print(n, "!=", result)
```
