---
layout: default
title: "Unit 2 Task 36 - Solution"
permalink: /tasks/2-36-solution/
---

# Solution - Task 36: Elevator floor hops

[← Back to task]({{ site.baseurl }}/tasks/2-36/)

---

One possible program:

```python
floor = 1

while True:
    target = int(input("Go to floor (0 to stop): "))
    if target == 0:
        break
    if target < 1:
        print("Invalid floor.")
        continue
    floor = target
    print("Now on floor", floor)

print("Elevator parked")
```
