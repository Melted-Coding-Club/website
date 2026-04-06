---
layout: default
title: "Unit 2 Task 38 - Solution"
permalink: /tasks/2-38-solution/
---

# Solution - Task 38: Live class average

[← Back to task]({{ site.baseurl }}/tasks/2-38/)

---

One possible program:

```python
total = 0.0
count = 0

while True:
    m = float(input("Mark (-1 to finish): "))
    if m == -1:
        print("Done")
        break
    if 0 <= m <= 100:
        count += 1
        total += m
        print("Running average:", total / count)
    else:
        print("Ignored - mark must be 0..100")
```
