---
layout: default
title: "Unit 2 Task 43 - Solution"
permalink: /tasks/2-43-solution/
---

# Solution - Task 43: Count digits in a sale ID

[← Back to task]({{ site.baseurl }}/tasks/2-43/)

---

One possible program:

```python
n = int(input("Positive ID: "))
digits = 0
x = n

while x > 0:
    x //= 10
    digits += 1

print("Digits:", digits)
```
