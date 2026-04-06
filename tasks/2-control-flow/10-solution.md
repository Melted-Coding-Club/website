---
layout: default
title: "Unit 2 Task 10 - Solution"
permalink: /tasks/2-control-flow/10-solution/
---

# Solution - Task 10: Sticker sheet total

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/10/)

---

One possible program:

```python
sheet_count = int(input("N (number of sheets): "))
total = 0

for sheet_number in range(1, sheet_count + 1):
    total += sheet_number

print("Total stickers:", total)
```
