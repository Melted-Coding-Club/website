---
layout: default
title: "Unit 3 Task 14 - Solution"
permalink: /tasks/3-14-solution/
---

# Solution - Task 14: Letter frequency

[← Back to task]({{ site.baseurl }}/tasks/3-14/)

---

One possible program:

```python
text = input("Word: ").strip().lower()
frequency = {}

for char in text:
    frequency[char] = frequency.get(char, 0) + 1

for char in frequency:
    print(char, ":", frequency[char])
```
