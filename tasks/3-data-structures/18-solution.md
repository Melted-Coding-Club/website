---
layout: default
title: "Unit 3 Task 18 - Solution"
permalink: /tasks/3-data-structures/18-solution/
---

# Solution - Task 18: Election-style tally

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/18/)

---

One possible program:

```python
options = ["pizza", "pasta", "salad"]
votes_list = []
tally = {"pizza": 0, "pasta": 0, "salad": 0}

while True:
    vote = input("Vote (pizza/pasta/salad or done): ").strip().lower()
    if vote == "done":
        break
    if vote not in tally:
        print("Invalid vote")
    else:
        votes_list.append(vote)
        tally[vote] = tally[vote] + 1

for choice in tally:
    print(choice, ":", tally[choice])

best_choice = options[0]
for choice in options:
    if tally[choice] > tally[best_choice]:
        best_choice = choice

print("Winner:", best_choice)
```
