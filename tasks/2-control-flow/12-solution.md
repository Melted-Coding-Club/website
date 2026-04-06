---
layout: default
title: "Unit 2 Task 12 - Solution"
permalink: /tasks/2-control-flow/12-solution/
---

# Solution - Task 12: Valid marks only

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/12/)

---

One possible program:

```python
total = 0.0
count = 0

while True:
    mark = float(input("Enter mark (-5 to finish): "))
    if mark == -5:
        break
    if 50 <= mark <= 100:
        count += 1
        total += mark

if count > 0:
    print("Average of valid marks:", total / count)
else:
    print("No valid marks entered.")
```
