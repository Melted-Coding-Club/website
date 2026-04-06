---
layout: default
title: "Unit 2 Task 25 - Solution"
permalink: /tasks/2-control-flow/25-solution/
---

# Solution - Task 25: Rock, paper, scissors - first to three

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/25/)

---

One possible program:

```python
import random

choices = ("r", "p", "s")
beats = {"r": "s", "s": "p", "p": "r"}

user_w = 0
cpu_w = 0

while user_w < 3 and cpu_w < 3:
    user_choice = input("Your play (r/p/s): ").lower().strip()
    while user_choice not in choices:
        user_choice = input("Type r, p, or s: ").lower().strip()
    computer_choice = random.choice(choices)
    print("Computer:", computer_choice)
    if user_choice == computer_choice:
        print("Tie - no point.")
    elif beats[user_choice] == computer_choice:
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
