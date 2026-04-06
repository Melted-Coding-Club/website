---
layout: default
title: "Unit 4 Task 11 - Solution"
permalink: /tasks/4-functions/11-solution/
---

# Solution - Task 11: Count divisors

[← Back to task]({{ site.baseurl }}/tasks/4-functions/11/)

---

One possible program:

```python
def count_divisors(n):
    c = 0
    for d in range(1, n + 1):
        if n % d == 0:
            c += 1
    return c

print(count_divisors(6))
```
