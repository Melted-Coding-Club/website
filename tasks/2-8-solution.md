---
layout: default
title: "Unit 2 Task 8 - Solution"
permalink: /tasks/2-8-solution/
---

# Solution - Task 8: Odd or even order total

[← Back to task]({{ site.baseurl }}/tasks/2-8/)

---

One possible program:

```python
n = int(input("Number of items: "))

if n % 2 == 0:
    print("Even - boxes pack evenly.")
else:
    print("Odd - one item left over.")
```
