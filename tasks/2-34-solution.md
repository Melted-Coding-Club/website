---
layout: default
title: "Unit 2 Task 34 - Solution"
permalink: /tasks/2-34-solution/
---

# Solution - Task 34: Simple pay-down balance

[← Back to task]({{ site.baseurl }}/tasks/2-34/)

---

One possible program:

```python
balance = float(input("Balance owed ($): "))
payment = float(input("Monthly payment ($): "))
months = 0

while balance > 0:
    balance -= payment
    months += 1

print("Paid off in", months, "months.")
```
