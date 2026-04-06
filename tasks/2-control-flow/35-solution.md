---
layout: default
title: "Unit 2 Task 35 - Solution"
permalink: /tasks/2-control-flow/35-solution/
---

# Solution - Task 35: Coffee stamp card

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/35/)

---

One possible program:

```python
stamps = 0
free_drinks = 0

while free_drinks < 2:
    stamps += 1
    print("Stamps:", stamps)
    if stamps == 10:
        print("Free coffee!")
        free_drinks += 1
        stamps = 0

print("Earned", free_drinks, "free drinks in this simulation.")
```
