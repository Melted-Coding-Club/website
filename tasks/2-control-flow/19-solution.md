---
layout: default
title: "Unit 2 Task 19 - Solution"
permalink: /tasks/2-control-flow/19-solution/
---

# Solution - Task 19: Shop times table poster

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/19/)

---

One possible program:

```python
pack_size = int(input("Pack size N: "))

for multiplier in range(1, 13):
    print(multiplier, "x", pack_size, "=", multiplier * pack_size)
```
