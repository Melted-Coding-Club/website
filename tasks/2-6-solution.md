---
layout: default
title: "Unit 2 Task 6 - Solution"
permalink: /tasks/2-6-solution/
---

# Solution - Task 6: Report card letter

[← Back to task]({{ site.baseurl }}/tasks/2-6/)

---

One possible program:

```python
mark = float(input("Course mark (%): "))

if mark >= 90:
    print("A")
elif mark >= 80:
    print("B")
elif mark >= 70:
    print("C")
elif mark >= 60:
    print("D")
else:
    print("F")
```
