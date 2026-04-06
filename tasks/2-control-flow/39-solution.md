---
layout: default
title: "Unit 2 Task 39 - Solution"
permalink: /tasks/2-control-flow/39-solution/
---

# Solution - Task 39: Café lunch order

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/39/)

---

One possible program:

```python
total = 0.0

while True:
    print("1. Sandwich $6  2. Soup $4  3. Drink $2  0. Done")
    choice = int(input("Choice: "))
    if choice == 0:
        break
    if choice == 1:
        total += 6
    elif choice == 2:
        total += 4
    elif choice == 3:
        total += 2
    else:
        print("Invalid choice")

print("Your total is $" + str(round(total, 2)))
```
