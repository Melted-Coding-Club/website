---
layout: default
title: "Unit 3 Task 15 - Solution"
permalink: /tasks/3-data-structures/15-solution/
---

# Solution - Task 15: Inventory commands

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/15/)

---

One possible program:

```python
inventory = {"pencil": 20, "eraser": 15}

while True:
    command = input("Command: ").strip()
    if command == "stop":
        break
    if command == "show":
        for product in inventory:
            print(product, inventory[product])
    elif command.startswith("add "):
        parts = command.split()
        product = parts[1]
        qty = int(parts[2])
        inventory[product] = inventory[product] + qty
```
