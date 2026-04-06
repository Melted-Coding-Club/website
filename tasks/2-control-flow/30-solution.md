---
layout: default
title: "Unit 2 Task 30 - Solution"
permalink: /tasks/2-control-flow/30-solution/
---

# Solution - Task 30: FizzBuzz inventory labels

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/30/)

---

One possible program:

```python
max_label = int(input("N: "))

for label_number in range(1, max_label + 1):
    if label_number % 3 == 0 and label_number % 5 == 0:
        print("FizzBuzz")
    elif label_number % 3 == 0:
        print("Fizz")
    elif label_number % 5 == 0:
        print("Buzz")
    else:
        print(label_number)
```
