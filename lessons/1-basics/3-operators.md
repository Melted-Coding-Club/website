---
layout: default
title: "1.3 Operators"
permalink: /lessons/1-basics/3-operators/
---

# 1.3 Operators

**Operators** are symbols that do something with values: maths, comparison, or logic.

## Maths operators

| Symbol | Meaning   | Example    |
|--------|-----------|------------|
| `+`    | Add       | `5 + 3` → 8 |
| `-`    | Subtract  | `5 - 3` → 2 |
| `*`    | Multiply  | `5 * 3` → 15 |
| `/`    | Divide    | `6 / 3` → 2.0 |
| `//`   | Divide (whole number) | `7 // 2` → 3 |
| `%`    | Remainder | `7 % 2` → 1 |

You can use variables too: `score * 2`, `health - 1`.

## Comparison operators

These compare two values and give `True` or `False`:

| Symbol | Meaning        | Example        |
|--------|----------------|----------------|
| `==`   | Equal to       | `5 == 5` → True |
| `!=`   | Not equal to   | `5 != 3` → True |
| `<`    | Less than      | `3 < 5` → True |
| `>`    | Greater than   | `10 > 7` → True |
| `<=`   | Less or equal  | `4 <= 4` → True |
| `>=`   | Greater or equal | `3 >= 3` → True |

Example:

```python
score = 10
print(score > 5)   # True
print(score == 10) # True
```

## Logical operators

- **`and`** - both sides must be True: `(age >= 10) and (age < 20)`
- **`or`** - at least one side True: `(score == 0) or (lives == 0)`
- **`not`** - flip True/False: `not game_over`

## Mini project: Simple calculator

Ask the user for two numbers (use `int(input(...))`). Then print:

- Their sum
- Their product (multiply)
- Whether the first is greater than the second (True or False)

---

**Navigation**

- **Previous:** [1.2 Variables]({{ site.baseurl }}/lessons/1-basics/2-variables/)
- **Next:** [2.1 Conditionals]({{ site.baseurl }}/lessons/2-control-flow/1-conditionals/)
- **All lessons:** [Lesson list on the homepage]({{ site.baseurl }}/)

**Tasks**

- [Unit 2 tasks]({{ site.baseurl }}/tasks/2/) - many problems use maths and comparisons (try after [2.1]({{ site.baseurl }}/lessons/2-control-flow/1-conditionals/) and [2.2]({{ site.baseurl }}/lessons/2-control-flow/2-loops/))

**Tutorial**

- [Tutorial 1.3]({{ site.baseurl }}/tutorials/1-3/) - guided project for this unit
