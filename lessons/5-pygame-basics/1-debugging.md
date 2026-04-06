---
layout: default
title: "5.1 Pygame setup and the game loop"
permalink: /lessons/5-pygame-basics/1-debugging/
---

# 5.1 Pygame setup and the game loop

We’re moving from text-based programs to a **game window**. Pygame is a library that gives you a window, shapes, colours, and keyboard input - everything you need for a simple game.

## Install Pygame

In the terminal (or your IDE’s terminal):

```bash
pip install pygame
```

If you use Python 3 specifically: `pip3 install pygame`.

## A minimal Pygame program

```python
import pygame

pygame.init()
screen = pygame.display.set_mode((400, 300))
pygame.display.set_caption("My Game")

running = True
while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    screen.fill((0, 0, 0))   # black background
    pygame.display.flip()     # show the new frame

pygame.quit()
```

- `pygame.init()` - start Pygame.
- `set_mode((width, height))` - open a window.
- **Game loop** - the `while running:` loop runs until the user closes the window.
- `pygame.event.get()` - list of things that happened (key press, mouse click, quit).
- `pygame.QUIT` - user clicked the close button.
- `screen.fill((r, g, b))` - paint the whole screen one colour. `(0, 0, 0)` is black.
- `pygame.display.flip()` - make the new frame visible.

## Important idea: you can’t “remove” shapes

In Pygame you don’t delete things from the screen. You **redraw the whole frame** every time. So each loop we:

1. Clear the screen (e.g. `screen.fill(...)`).
2. Draw everything that should be visible (player, obstacles, etc.).
3. Call `pygame.display.flip()`.

Anything you drew last time is gone after the fill; only what you draw this time appears.

## Project: Empty game window

1. Create a new file and run the minimal program above.
2. Change the window size and the background colour (try `(30, 60, 100)` for a blue).
3. Close the window with the X and confirm the program exits cleanly.

---

**Navigation**

- **Previous:** [4.2 Scope and return values]({{ site.baseurl }}/lessons/4-functions/2-scope-and-return-values/)
- **Next:** [5.2 Coordinates and drawing]({{ site.baseurl }}/lessons/5-pygame-basics/2-projects/)
- **All lessons:** [Lesson list on the homepage]({{ site.baseurl }}/)

**Tasks**

- [Unit 2 tasks]({{ site.baseurl }}/tasks/2-control-flow/) - text-based Python practice (Pygame builds on the same ideas: loops, events, state)

**Tutorial**

- [Tutorial 5.1]({{ site.baseurl }}/tutorials/5-1/) - guided steps for this unit

**Resources**

- [Resources: Python, Pygame, and more]({{ site.baseurl }}/resources/) - install tips and documentation links
