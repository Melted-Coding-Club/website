---
layout: default
title: "4.2 Scope and return values"
permalink: /lessons/4-functions/2-scope-and-return-values/
---

# 4.2 Scope and return values

**Scope** means where a variable is visible. **Return values** let functions send results back so the rest of the program can use them.

## Scope: local vs global

Variables created **inside** a function are **local**: they only exist in that function.

```python
def set_score():
    score = 100
    print(score)  # 100

set_score()
print(score)  # Error! score doesn't exist here
```

Variables defined **outside** functions (at the top of the file) are **global** and can be read inside functions. But if you assign to that name inside a function, you create a **new** local variable unless you use `global` (which we’ll avoid for now). So: prefer **passing values in** and **returning values out** instead of global variables.

## Passing data in, getting data out

- **Parameters** pass data in.
- **Return** passes data out.

Example:

```python
def add(a, b):
    total = a + b
    return total

x = add(3, 5)   # x is 8
print(add(10, 2))  # 12
```

You can return more than one value: `return score, lives` and then `s, l = get_state()`.

## Returning early

You can use `return` in the middle of a function to exit early:

```python
def is_positive(n):
    if n <= 0:
        return False
    return True
```

## A quick debugging tip

When something goes wrong:

1. Add `print(...)` to see what values variables have.
2. Check your **indentation** - wrong indent can cause logic errors or "unexpected indent" messages.
3. Read the error message: it often says which line and what went wrong (e.g. "name 'x' is not defined" means you used a variable that doesn’t exist in that scope).

## Mini project: Helper functions

Write a small game or quiz that uses at least two functions that **return** values, e.g.:

- `roll_dice()` returns a random number 1–6.
- `ask_question(question, answer)` returns True if the user’s input matches the answer, else False.

Use the return values in your main loop to update score or state.

---

**Navigation**

- **Previous:** [4.1 Defining functions]({{ site.baseurl }}/lessons/4-functions/1-defining-functions/)
- **Next:** [5.1 Pygame setup and the game loop]({{ site.baseurl }}/lessons/5-pygame-basics/1-debugging/)
- **All lessons:** [Lesson list on the homepage]({{ site.baseurl }}/)

**Tasks**

- [Unit 3 tasks]({{ site.baseurl }}/tasks/3/) - refactor list and dictionary programs with small functions that return values
- [Unit 2 tasks]({{ site.baseurl }}/tasks/2/) - shorter programs for return values and control flow before Pygame

**Tutorial**

- [Tutorial 4.2]({{ site.baseurl }}/tutorials/4-2/) - guided project for this unit
