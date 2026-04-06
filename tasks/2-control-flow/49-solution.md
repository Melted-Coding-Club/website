---
layout: default
title: "Unit 2 Task 49 - Solution"
permalink: /tasks/2-control-flow/49-solution/
---

# Solution - Task 49: Full multiplication square

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/49/)

---

One possible program:

```python
for row in range(1, 13):
    for col in range(1, 13):
        print(row * col, end="\t")
    print()
```
