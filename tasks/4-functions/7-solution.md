---
layout: default
title: "Unit 4 Task 7 - Solution"
permalink: /tasks/4-functions/7-solution/
---

# Solution - Task 7: Is it a vowel?

[← Back to task]({{ site.baseurl }}/tasks/4-functions/7/)

---

One possible program:

```python
def is_vowel(ch):
    return ch.lower() in "aeiou"

print(is_vowel("A"))
print(is_vowel("x"))
```
