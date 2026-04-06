---
layout: default
title: "Unit 2 Task 29 - Solution"
permalink: /tasks/2-control-flow/29-solution/
---

# Solution - Task 29: Bus passenger count

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/29/)

---

One possible program:

```python
passengers = 0

while True:
    change = int(input("Board (+) or alight (-) count (0 to end): "))
    if change == 0:
        break
    if change > 0:
        passengers += change
    else:
        leave = -change
        passengers -= leave
        if passengers < 0:
            passengers = 0

print("Final passengers on board:", passengers)
```
