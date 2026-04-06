---
layout: default
title: "Unit 2 Task 14 - Solution"
permalink: /tasks/2-14-solution/
---

# Solution - Task 14: Coin race to ten

[← Back to task]({{ site.baseurl }}/tasks/2-14/)

---

One possible program:

```python
import random

heads_count = 0
tails_count = 0

while heads_count < 10 and tails_count < 10:
    coin = random.randint(0, 1)
    if coin == 0:
        print("Tails")
        tails_count += 1
    else:
        print("Heads")
        heads_count += 1

if tails_count > heads_count:
    print("Tails Wins!")
else:
    print("Heads Wins!")
print("Total flips:", heads_count + tails_count)
```
