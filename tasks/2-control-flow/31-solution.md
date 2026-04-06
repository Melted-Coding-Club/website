---
layout: default
title: "Unit 2 Task 31 - Solution"
permalink: /tasks/2-control-flow/31-solution/
---

# Solution - Task 31: Is this number prime?

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/31/)

---

One possible program:

```python
number_to_check = int(input("n (>=2): "))
is_prime = True

for divisor in range(2, number_to_check):
    if number_to_check % divisor == 0:
        is_prime = False
        break

if is_prime:
    print("prime")
else:
    print("not prime")
```
