---
layout: default
title: "Unit 2 Task 44 - Solution"
permalink: /tasks/2-44-solution/
---

# Solution - Task 44: Reverse digits of a sale code

[← Back to task]({{ site.baseurl }}/tasks/2-44/)

---

One possible program:

```python
original_code = int(input("Positive code: "))
reversed_code = 0
remaining = original_code

while remaining > 0:
    reversed_code = reversed_code * 10 + (remaining % 10)
    remaining //= 10

print("Reversed:", reversed_code)
```
