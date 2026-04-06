---
layout: default
title: "Unit 2 Task 20 - Solution"
permalink: /tasks/2-control-flow/20-solution/
---

# Solution - Task 20: Factorial orderings

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/20/)

---

One possible program:

```python
factorial_input = int(input("N: "))
result = 1

for factor in range(1, factorial_input + 1):
    result *= factor

print(factorial_input, "!=", result)
```
