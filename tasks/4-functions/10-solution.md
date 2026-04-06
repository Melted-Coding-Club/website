---
layout: default
title: "Unit 4 Task 10 - Solution"
permalink: /tasks/4-functions/10-solution/
---

# Solution - Task 10: Sum from 1 to n

[← Back to task]({{ site.baseurl }}/tasks/4-functions/10/)

---

One possible program:

```python
def sum_to(n):
    total = 0
    for i in range(1, n + 1):
        total += i
    return total

print(sum_to(10))
```
