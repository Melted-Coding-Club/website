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
first = int(input("First number: "))
second = int(input("Second number: "))

while second != 0:
    first, second = second, first % second

print("GCD is", first)
```
