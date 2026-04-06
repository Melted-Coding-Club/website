---
layout: default
title: "Unit 2 Task 16 - Solution"
permalink: /tasks/2-control-flow/16-solution/
---

# Solution - Task 16: ATM PIN (three tries)

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/16/)

---

One possible program:

```python
correct = "2468"
attempts_left = 3

while attempts_left > 0:
    pin = input("Enter PIN: ")
    if pin == correct:
        print("Welcome")
        break
    attempts_left -= 1
    if attempts_left > 0:
        print("Wrong. Tries left:", attempts_left)
    else:
        print("Card locked")
```
