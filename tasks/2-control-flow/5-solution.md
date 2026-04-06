---
layout: default
title: "Unit 2 Task 5 - Solution"
permalink: /tasks/2-control-flow/5-solution/
---

# Solution - Task 5: Zoo ticket price

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/5/)

---

One possible program:

```python
age = int(input("Visitor age: "))

if age < 13:
    print("Child ticket: $8")
elif age >= 65:
    print("Senior ticket: $10")
else:
    print("Adult ticket: $15")
```
