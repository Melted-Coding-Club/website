---
layout: default
title: "Unit 2 Task 9 - Solution"
permalink: /tasks/2-control-flow/9-solution/
---

# Solution - Task 9: Bus departure countdown

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/9/)

---

One possible program:

```python
minutes_until_departure = int(input("Minutes until departure: "))

for remaining_minutes in range(minutes_until_departure, 0, -1):
    print(remaining_minutes)
```
