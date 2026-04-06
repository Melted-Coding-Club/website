---
layout: default
title: "Unit 2 Task 41 - Solution"
permalink: /tasks/2-41-solution/
---

# Solution - Task 41: Greatest common divisor

[← Back to task]({{ site.baseurl }}/tasks/2-41/)

---

One possible program:

```python
a = int(input("a: "))
b = int(input("b: "))

while b != 0:
    a, b = b, a % b

print("GCD is", a)
```
