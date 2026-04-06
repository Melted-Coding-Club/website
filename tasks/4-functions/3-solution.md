---
layout: default
title: "Unit 4 Task 3 - Solution"
permalink: /tasks/4-functions/3-solution/
---

# Solution - Task 3: Price after discount

[← Back to task]({{ site.baseurl }}/tasks/4-functions/3/)

---

One possible program:

```python
def discounted_price(price, percent_off):
    return price * (1 - percent_off / 100)

print(discounted_price(100.0, 20))
print(discounted_price(50.0, 10))
```
