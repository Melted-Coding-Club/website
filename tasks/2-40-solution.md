---
layout: default
title: "Unit 2 Task 40 - Solution"
permalink: /tasks/2-40-solution/
---

# Solution - Task 40: Fibonacci rabbit pairs (small n)

[← Back to task]({{ site.baseurl }}/tasks/2-40/)

---

One possible program:

```python
n = int(input("How many Fibonacci terms: "))
a, b = 1, 1

for i in range(n):
    print(a)
    a, b = b, a + b
```
