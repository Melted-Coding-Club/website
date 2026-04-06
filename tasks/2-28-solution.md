---
layout: default
title: "Unit 2 Task 28 - Solution"
permalink: /tasks/2-28-solution/
---

# Solution - Task 28: Stock on the shelf

[← Back to task]({{ site.baseurl }}/tasks/2-28/)

---

One possible program:

```python
stock = int(input("Starting stock: "))

while stock > 0:
    sold = int(input("Items sold this hour (0 to close): "))
    if sold == 0:
        print("Closing. Stock left:", stock)
        break
    if sold > stock:
        print("Not enough stock")
    else:
        stock -= sold
        print("Stock left:", stock)

if stock == 0:
    print("Shelf empty")
```
