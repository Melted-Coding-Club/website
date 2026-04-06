---
layout: default
title: "Unit 2 Task 10 - Solution"
permalink: /tasks/2-10-solution/
---

# Solution - Task 10: Sticker sheet total

[← Back to task]({{ site.baseurl }}/tasks/2-10/)

---

One possible program:

```python
n = int(input("N (number of sheets): "))
total = 0

for i in range(1, n + 1):
    total += i

print("Total stickers:", total)
```
