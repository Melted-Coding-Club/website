---
layout: default
title: "Unit 2 Task 30 - Solution"
permalink: /tasks/2-30-solution/
---

# Solution - Task 30: FizzBuzz inventory labels

[← Back to task]({{ site.baseurl }}/tasks/2-30/)

---

One possible program:

```python
n = int(input("N: "))

for i in range(1, n + 1):
    if i % 3 == 0 and i % 5 == 0:
        print("FizzBuzz")
    elif i % 3 == 0:
        print("Fizz")
    elif i % 5 == 0:
        print("Buzz")
    else:
        print(i)
```
