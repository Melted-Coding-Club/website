---
layout: default
title: "Unit 2 Task 46 - Solution"
permalink: /tasks/2-control-flow/46-solution/
---

# Solution - Task 46: Guess my number with play again

[← Back to task]({{ site.baseurl }}/tasks/2-control-flow/46/)

---

One possible program:

```python
import random

play_again = "y"
while play_again.lower() == "y":
    secret = random.randint(1, 20)
    print("New game! 1-20.")
    while True:
        player_guess = int(input("Guess: "))
        if player_guess < secret:
            print("Too low")
        elif player_guess > secret:
            print("Too high")
        else:
            print("Got it!")
            break
    play_again = input("Play again? (y/n): ")
```
