---
layout: default
title: "Unit 2 Task 9 - Solution"
permalink: /tasks/2-9-solution/
---

# Solution - Task 9: Bus departure countdown

[← Back to task]({{ site.baseurl }}/tasks/2-9/)

---

One possible program:

```python
n = int(input("Minutes until departure: "))

for m in range(n, 0, -1):
    print(m)
```
