---
layout: default
title: "Unit 2 Task 45 - Solution"
permalink: /tasks/2-control-flow/45-solution/
---

# Solution - Task 45: Sum of squares pyramid

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/45/)

---

One possible program:

```python
layer_count = int(input("n: "))
total = 0

for layer in range(1, layer_count + 1):
    total += layer * layer

print("Sum of squares:", total)
```
