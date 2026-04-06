---
layout: default
title: "Unit 2 Task 43 - Solution"
permalink: /tasks/2-control-flow/43-solution/
---

# Solution - Task 43: Count digits in a sale ID

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/43/)

---

One possible program:

```python
sale_id = int(input("Positive ID: "))
digits = 0
remaining = sale_id

while remaining > 0:
    remaining //= 10
    digits += 1

print("Digits:", digits)
```
