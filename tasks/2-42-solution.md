---
layout: default
title: "Unit 2 Task 42 - Solution"
permalink: /tasks/2-42-solution/
---

# Solution - Task 42: Powers by repeated multiplication

[← Back to task]({{ site.baseurl }}/tasks/2-42/)

---

One possible program:

```python
base = int(input("base: "))
exp = int(input("exponent (>=0): "))
result = 1

for repeat in range(exp):
    result *= base

print(result)
```
