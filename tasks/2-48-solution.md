---
layout: default
title: "Unit 2 Task 48 - Solution"
permalink: /tasks/2-48-solution/
---

# Solution - Task 48: Star triangle banner

[← Back to task]({{ site.baseurl }}/tasks/2-48/)

---

One possible program:

```python
n = int(input("Rows: "))

for row in range(1, n + 1):
    print("*" * row)
```
