---
layout: default
title: "Unit 3 Task 7 - Solution"
permalink: /tasks/3-7-solution/
---

# Solution - Task 7: Cheapest item index

[← Back to task]({{ site.baseurl }}/tasks/3-7/)

---

One possible program:

```python
prices = []

for slot in range(5):
    price = float(input("Price " + str(slot + 1) + ": "))
    prices.append(price)

best_index = 0
for index in range(1, len(prices)):
    if prices[index] < prices[best_index]:
        best_index = index

print("Cheapest item is number", best_index + 1, "at price", prices[best_index])
```
