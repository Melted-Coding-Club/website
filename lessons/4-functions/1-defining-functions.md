---
layout: default
title: "4.1 Defining functions"
permalink: /lessons/4-functions/1-defining-functions/
---

# 4.1 Defining functions

A **function** is a named block of code you can run whenever you need it. That keeps your program tidy and avoids repeating the same code.

## Defining a function

Use `def`, the function name, brackets, and a colon. The code that runs when you call the function is indented:

```python
def say_hello():
    print("Hello!")
    print("Welcome to coding club.")
```

## Calling a function

Use the name and brackets:

```python
say_hello()
say_hello()
```

Each call runs the whole block.

## Parameters (inputs)

You can pass **arguments** into the function. The names in the brackets are **parameters**:

```python
def greet(name):
    print("Hello,", name)

greet("Alex")
greet("Sam")
```

You can have several parameters: `def add(a, b):` then `add(3, 5)`.

## Return values

Use `return` to send a value back. The caller can use it in an expression or assign it:

```python
def double(n):
    return n * 2

result = double(5)   # result is 10
print(double(7))    # 14
```

After a `return`, the function stops. Code below it in the same function won’t run.

## Mini project: Refactor the guessing game

Take your Higher–Lower game and split it into functions, for example:

- `get_guess()` - asks for a number and returns it (with a loop until they type a valid number if you like).
- `check_guess(guess, secret)` - returns `"high"`, `"low"` or `"correct"`.
- `main()` - picks `secret`, loops until correct, calls `get_guess()` and `check_guess()`, prints the message.

Then at the bottom: `main()`.

---

**Navigation**

- **Previous:** [3.2 Dictionaries and objects]({{ site.baseurl }}/lessons/3-data-structures/2-dictionaries-and-objects/)
- **Next:** [4.2 Scope and return values]({{ site.baseurl }}/lessons/4-functions/2-scope-and-return-values/)
- **All lessons:** [Lesson list on the homepage]({{ site.baseurl }}/)

**Tasks**

- [Unit 3 tasks]({{ site.baseurl }}/tasks/3/) - good candidates to refactor with `def` once you know functions
- [Unit 2 tasks]({{ site.baseurl }}/tasks/2/) - shorter programs for practising `def` and `return`

**Tutorial**

- [Tutorial 4.1]({{ site.baseurl }}/tutorials/4-1/) - guided project for this unit
