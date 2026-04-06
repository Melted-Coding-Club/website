---
layout: default
title: "Unit 3 Task 17 - Solution"
permalink: /tasks/3-data-structures/17-solution/
---

# Solution - Task 17: Simple phrasebook

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/17/)

---

One possible program:

```python
phrasebook = {
    "hello": "hola",
    "yes": "si",
    "no": "no",
    "water": "agua",
    "thanks": "gracias",
}

while True:
    english = input("English word (or 'quit'): ").strip().lower()
    if english == "quit":
        break
    print(phrasebook.get(english, "No translation"))
```
