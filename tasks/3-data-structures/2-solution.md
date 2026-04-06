---
layout: default
title: "Unit 3 Task 2 - Solution"
permalink: /tasks/3-data-structures/2-solution/
---

# Solution - Task 2: Lap times summary

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/2/)

---

One possible program:

```python
lap_times = [58.2, 57.1, 59.0, 57.8, 56.9]

fastest = min(lap_times)
average = sum(lap_times) / len(lap_times)

print("Fastest lap (s):", fastest)
print("Average lap (s):", average)
```
