---
layout: default
title: "Unit 2 Task 31 - Solution"
permalink: /tasks/2-31-solution/
---

# Solution - Task 31: Is this number prime?

[← Back to task]({{ site.baseurl }}/tasks/2-31/)

---

One possible program:

```python
n = int(input("n (>=2): "))
is_prime = True

for d in range(2, n):
    if n % d == 0:
        is_prime = False
        break

if is_prime:
    print("prime")
else:
    print("not prime")
```
