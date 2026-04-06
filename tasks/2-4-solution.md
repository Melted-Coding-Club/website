---
layout: default
title: "Unit 2 Task 4 - Solution"
permalink: /tasks/2-4-solution/
---

# Solution - Task 4: Counting even raffle tickets

[← Back to task]({{ site.baseurl }}/tasks/2-4/)

---

One possible program:

```python
count = 0

while True:
    num = int(input("Enter ticket number (-1 to stop): "))
    if num == -1:
        break
    if num % 2 == 0:
        count += 1

print("Even ticket numbers entered:", count)
```
