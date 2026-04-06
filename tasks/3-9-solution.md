---
layout: default
title: "Unit 3 Task 9 - Solution"
permalink: /tasks/3-9-solution/
---

# Solution - Task 9: Merge two stock shelves

[← Back to task]({{ site.baseurl }}/tasks/3-9/)

---

One possible program:

```python
shelf_a = [10, 5, 8]
shelf_b = [3, 12, 4]
combined = []

for index in range(len(shelf_a)):
    combined.append(shelf_a[index] + shelf_b[index])

print("Shelf A:", shelf_a)
print("Shelf B:", shelf_b)
print("Combined:", combined)
```
