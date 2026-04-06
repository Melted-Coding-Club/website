---
layout: default
title: "Unit 2 Task 7 - Solution"
permalink: /tasks/2-7-solution/
---

# Solution - Task 7: Freezing day on the farm

[← Back to task]({{ site.baseurl }}/tasks/2-7/)

---

One possible program:

```python
t = float(input("Morning temperature (C): "))

if t <= 0:
    print("At or below freezing - ice is possible.")
else:
    print("Above freezing.")
```
