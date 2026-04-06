---
layout: default
title: "Unit 3 Task 8 - Solution"
permalink: /tasks/3-8-solution/
---

# Solution - Task 8: Double every level score

[← Back to task]({{ site.baseurl }}/tasks/3-8/)

---

One possible program:

```python
level_scores = [100, 250, 400, 120]
doubled_scores = []

for score in level_scores:
    doubled_scores.append(score * 2)

print("Original:", level_scores)
print("Doubled: ", doubled_scores)
```
