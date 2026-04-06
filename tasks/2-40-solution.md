---
layout: default
title: "Unit 2 Task 40 - Solution"
permalink: /tasks/2-40-solution/
---

# Solution - Task 40: Fibonacci rabbit pairs (small n)

[← Back to task]({{ site.baseurl }}/tasks/2-40/)

---

One possible program:

```python
term_count = int(input("How many Fibonacci terms: "))
previous_term = 1
current_term = 1

for term_index in range(term_count):
    print(previous_term)
    previous_term, current_term = current_term, previous_term + current_term
```
