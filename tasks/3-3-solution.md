---
layout: default
title: "Unit 3 Task 3 - Solution"
permalink: /tasks/3-3-solution/
---

# Solution - Task 3: Build a playlist

[← Back to task]({{ site.baseurl }}/tasks/3-3/)

---

One possible program:

```python
playlist = []

while True:
    title = input("Song title (blank to finish): ")
    if title == "":
        break
    playlist.append(title)

print("Playlist has", len(playlist), "song(s):")
for index in range(len(playlist)):
    print(str(index + 1) + ".", playlist[index])
```
