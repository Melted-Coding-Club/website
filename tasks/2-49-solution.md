---
layout: default
title: "Unit 2 Task 49 - Solution"
permalink: /tasks/2-49-solution/
---

# Solution - Task 49: Full multiplication square

[← Back to task]({{ site.baseurl }}/tasks/2-49/)

---

One possible program:

```python
for r in range(1, 13):
    for c in range(1, 13):
        print(r * c, end="\t")
    print()
```
