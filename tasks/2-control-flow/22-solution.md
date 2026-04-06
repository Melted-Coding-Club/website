---
layout: default
title: "Unit 2 Task 22 - Solution"
permalink: /tasks/2-control-flow/22-solution/
---

# Solution - Task 22: Savings goal

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/22/)

---

One possible program:

```python
goal = float(input("Savings goal ($): "))
balance = 0.0
weeks = 0

while balance < goal:
    weekly_savings = float(input("Saved this week ($): "))
    balance += weekly_savings
    weeks += 1

print("Goal reached in", weeks, "weeks. Balance:", balance)
```
