---
layout: default
title: "2.1 Conditionals"
permalink: /lessons/2-control-flow/1-conditionals/
---

# 2.1 Conditionals

**Conditionals** let your program make decisions: run one block of code when something is true, and a different block when it’s false.

## if

Use `if` and a condition. The code that runs when the condition is true is **indented** (usually 4 spaces):

```python
score = 50
if score >= 50:
    print("You passed!")
```

If `score` were 30, nothing would print. Only when `score >= 50` is True does the indented code run.

## Indentation matters

In Python, indentation shows which lines belong to the `if`. Everything that’s indented under `if` runs only when the condition is True.

```python
if score > 0:
    print("Score is positive")
    print("Well done")
print("This always runs")  # not indented, so not part of the if
```

## else

Use `else` to run code when the condition is **not** true:

```python
age = 12
if age >= 13:
    print("You can join")
else:
    print("Come back when you're 13")
```

## elif (else if)

Use `elif` to check another condition when the first one was false:

```python
score = 75
if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("Keep practising")
```

Only one of these blocks runs: the first condition that is True.

## Mini project: Secret number (one guess)

1. Choose a secret number and store it in a variable.
2. Use `input()` to get the user’s guess (convert to `int`).
3. Use `if`, `elif` and `else` to print "Too high!", "Too low!" or "Correct!".
4. (In the next lesson we’ll add a loop so they can keep guessing.)

---

**Navigation**

- **Previous:** [1.3 Operators]({{ site.baseurl }}/lessons/1-basics/3-operators/)
- **Next:** [2.2 Loops]({{ site.baseurl }}/lessons/2-control-flow/2-loops/)
- **All lessons:** [Lesson list on the homepage]({{ site.baseurl }}/)

**Tasks**

- [Unit 2 tasks]({{ site.baseurl }}/tasks/2/) - lots of practice with `if`, `elif`, and `else` (e.g. menus, grades, tickets; loops come in too on many pages)

**Tutorial**

- [Tutorial 2.1]({{ site.baseurl }}/tutorials/2-1/) - guided project for this unit
