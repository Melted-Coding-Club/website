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
n = int(input("Positive code: "))
rev = 0
x = n

while x > 0:
    rev = rev * 10 + (x % 10)
    x //= 10

print("Reversed:", rev)
```
