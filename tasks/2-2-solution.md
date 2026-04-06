---
layout: default
title: "Unit 2 Task 2 - Solution"
permalink: /tasks/2-2-solution/
---

# Solution - Task 2: Highest temperature this week

[← Back to task]({{ site.baseurl }}/tasks/2-2/)

---

One possible program:

```python
largest = None

for day_index in range(5):
    temp = float(input("Enter high temperature (C): "))
    if largest is None or temp > largest:
        largest = temp

print("Largest high temperature:", largest)
```
