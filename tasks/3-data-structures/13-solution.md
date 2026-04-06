---
layout: default
title: "Unit 3 Task 13 - Solution"
permalink: /tasks/3-data-structures/13-solution/
---

# Solution - Task 13: Word tally from a sentence

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/13/)

---

One possible program:

```python
line = input("Enter a sentence: ")
words = line.split()
counts = {}

for word in words:
    counts[word] = counts.get(word, 0) + 1

for word in counts:
    print(word, ":", counts[word])
```
