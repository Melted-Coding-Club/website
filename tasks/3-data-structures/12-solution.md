---
layout: default
title: "Unit 3 Task 12 - Solution"
permalink: /tasks/3-data-structures/12-solution/
---

# Solution - Task 12: Capital city lookup

[← Back to task]({{ site.baseurl }}/tasks/3-data-structures/12/)

---

One possible program:

```python
capitals = {
    "france": "Paris",
    "japan": "Tokyo",
    "egypt": "Cairo",
    "brazil": "Brasilia",
}

while True:
    country = input("Country (or 'quit'): ").strip().lower()
    if country == "quit":
        break
    city = capitals.get(country)
    if city is None:
        print("Unknown country")
    else:
        print(city)
```
