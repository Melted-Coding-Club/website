---
layout: default
title: "Unit 2 Task 19 - Solution"
permalink: /tasks/2-19-solution/
---

# Solution - Task 19: Shop times table poster

[← Back to task]({{ site.baseurl }}/tasks/2-19/)

---

One possible program:

```python
n = int(input("Pack size N: "))

for k in range(1, 13):
    print(k, "x", n, "=", k * n)
```
