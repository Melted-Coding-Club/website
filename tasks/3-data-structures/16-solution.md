---
layout: default
title: "Unit 3 Task 16 - Solution"
permalink: /tasks/3-data-structures/16-solution/
---

# Solution - Task 16: Attendance tally

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/16/)

---

One possible program:

```python
attendance = {}

while True:
    name = input("Student name (or 'done'): ").strip()
    if name.lower() == "done":
        break
    if name in attendance:
        attendance[name] = attendance[name] + 1
    else:
        attendance[name] = 1

for name in attendance:
    print(name, ":", attendance[name], "day(s)")
```
