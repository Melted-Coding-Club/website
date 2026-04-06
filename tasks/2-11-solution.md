---
layout: default
title: "Unit 2 Task 11 - Solution"
permalink: /tasks/2-11-solution/
---

# Solution - Task 11: Strawberry stand checkout

[← Back to task]({{ site.baseurl }}/tasks/2-11/)

---

One possible program:

```python
cost = float(input("Enter the cost: "))
money = float(input("Enter money from customer: "))

while money < cost:
    print("No sale")
    money = float(input("Enter money from customer: "))

if money == cost:
    print("Thank you for your payment")
else:
    change = round(money - cost, 1)
    print("Your change is: $" + str(change))
```
