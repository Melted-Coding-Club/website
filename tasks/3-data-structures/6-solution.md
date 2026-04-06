---
layout: default
title: "Unit 3 Task 6 - Solution"
permalink: /tasks/3-data-structures/6-solution/
---

# Solution - Task 6: Team roster

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/6/)

---

One possible program:

```python
roster = []

while True:
    player = input("Player name (or 'done'): ").strip()
    if player.lower() == "done":
        break
    roster.append(player)

print("Team has", len(roster), "players:")
for name in roster:
    print(name)
```
