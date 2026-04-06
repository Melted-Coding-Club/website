---
layout: default
title: "Unit 3 Task 5 - Solution"
permalink: /tasks/3-data-structures/5-solution/
---

# Solution - Task 5: Unique sign-up list

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/5/)

---

One possible program:

```python
names_list = []

while True:
    name = input("Name (or 'done'): ").strip()
    if name.lower() == "done":
        break
    if name in names_list:
        print("Already signed up")
    else:
        names_list.append(name)

print("Sign-ups:")
for person in names_list:
    print(person)
```
