---
layout: default
title: "Unit 4 Task 9 - Solution"
permalink: /tasks/4-functions/9-solution/
---

# Solution - Task 9: Small factorial

[← Back to task]({{ site.baseurl }}/tasks/4-functions/9/)

---

One possible program:

```python
def factorial(n):
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result

print(factorial(5))
```
