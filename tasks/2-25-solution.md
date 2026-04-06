---
layout: default
title: "Unit 2 Task 25 - Solution"
permalink: /tasks/2-25-solution/
---

# Solution - Task 25: Rock, paper, scissors - first to three

[← Back to task]({{ site.baseurl }}/tasks/2-25/)

---

One possible program:

```python
import random

choices = ("r", "p", "s")
beats = {"r": "s", "s": "p", "p": "r"}

user_w = 0
cpu_w = 0

while user_w < 3 and cpu_w < 3:
    u = input("Your play (r/p/s): ").lower().strip()
    while u not in choices:
        u = input("Type r, p, or s: ").lower().strip()
    c = random.choice(choices)
    print("Computer:", c)
    if u == c:
        print("Tie - no point.")
    elif beats[u] == c:
        print("You win the round.")
        user_w += 1
    else:
        print("Computer wins the round.")
        cpu_w += 1
    print("Score - you:", user_w, "computer:", cpu_w)

if user_w > cpu_w:
    print("You win the match!")
else:
    print("Computer wins the match!")
```
