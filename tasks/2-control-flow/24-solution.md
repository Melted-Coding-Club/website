---
layout: default
title: "Unit 2 Task 24 - Solution"
permalink: /tasks/2-control-flow/24-solution/
---

# Solution - Task 24: Guess with seven tries

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/24/)

---

One possible program:

```python
import random

secret = random.randint(1, 50)
print("Guess my number from 1 to 50. You have 7 tries.")

for attempt in range(7):
    guess = int(input("Guess: "))
    if guess == secret:
        print("You got it!")
        break
    if guess < secret:
        print("Too low")
    else:
        print("Too high")
else:
    print("You lose. The number was", secret)
```
