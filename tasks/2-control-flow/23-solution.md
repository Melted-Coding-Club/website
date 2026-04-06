---
layout: default
title: "Unit 2 Task 23 - Solution"
permalink: /tasks/2-control-flow/23-solution/
---

# Solution - Task 23: Strong enough Wi‑Fi password

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/23/)

---

One possible program:

```python
password = input("Choose a password: ")

while len(password) < 8:
    print("Too short - need at least 8 characters.")
    password = input("Choose a password: ")

print("Password accepted")
```
