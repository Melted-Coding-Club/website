---
layout: default
title: "Unit 2 Task 46 - Solution"
permalink: /tasks/2-46-solution/
---

# Solution - Task 46: Guess my number with play again

[← Back to task]({{ site.baseurl }}/tasks/2-46/)

---

One possible program:

```python
import random

play = "y"
while play.lower() == "y":
    secret = random.randint(1, 20)
    print("New game! 1-20.")
    while True:
        g = int(input("Guess: "))
        if g < secret:
            print("Too low")
        elif g > secret:
            print("Too high")
        else:
            print("Got it!")
            break
    play = input("Play again? (y/n): ")
```
