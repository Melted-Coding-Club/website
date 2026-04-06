---
layout: default
title: "Unit 3 Task 4 - Solution"
permalink: /tasks/3-data-structures/4-solution/
---

# Solution - Task 4: Marks in a list

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/4/)

---

One possible program:

```python
marks = []

while True:
    mark = float(input("Mark (-1 to finish): "))
    if mark == -1:
        break
    marks.append(mark)

if len(marks) == 0:
    print("No marks entered.")
else:
    print("Count:", len(marks))
    print("Average:", sum(marks) / len(marks))
```
