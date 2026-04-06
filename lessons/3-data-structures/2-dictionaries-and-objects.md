---
layout: default
title: "3.2 Dictionaries and objects"
permalink: /lessons/3-data-structures/2-dictionaries-and-objects/
---

# 3.2 Dictionaries and objects

A **dictionary** stores **key–value** pairs. Like a real dictionary: you look up a word (the key) and get its meaning (the value).

## Why "dictionary"?

In a real dictionary you have:

- **cookie** → "a baked snack"
- **variable** → "a name for a value in code"

In Python we do the same: each **key** has one **value**.

## Creating a dictionary

Use curly braces. Each pair is `"key": value`:

```python
glossary = {"cookie": "a baked snack", "variable": "a name for a value in code"}
```

So `glossary["cookie"]` gives `"a baked snack"`.

## Getting a value

Use the key in square brackets:

```python
dictionary = {"cookie": "a baked snack"}
print(dictionary["cookie"])   # a baked snack
```

If the key doesn’t exist, you get an error. You can avoid that with `.get()`: `dictionary.get("missing")` returns `None` (or a default you choose).

## Adding and changing

- Add or change: `dictionary["new_key"] = "new value"`
- Keys are often strings; values can be anything: numbers, strings, lists, even other dicts.

## Example: word lookup

```python
words = {"hello": "a greeting", "loop": "code that repeats", "bug": "an error in code"}
word = input("Enter a word: ")
if word in words:
    print(words[word])
else:
    print("Not in dictionary")
```

## Mini project: Glossary quiz

1. Make a dictionary of 5 programming words and their definitions.
2. Use a loop to ask the user for a word.
3. If the word is in the dictionary, print its definition; otherwise say "Unknown".
4. (Optional: pick a random key with `import random` and `random.choice(list(words.keys()))` and ask "What does X mean?")

---

**Navigation**

- **Previous:** [3.1 Lists and arrays]({{ site.baseurl }}/lessons/3-data-structures/1-lists-and-arrays/)
- **Next:** [4.1 Defining functions]({{ site.baseurl }}/lessons/4-functions/1-defining-functions/)
- **All lessons:** [Lesson list on the homepage]({{ site.baseurl }}/)

**Tasks**

- [Unit 3 tasks]({{ site.baseurl }}/tasks/3-data-structures/) - dictionaries, counting, and list-plus-dict problems (tasks 11 onward focus on dicts)
- [Unit 2 tasks]({{ site.baseurl }}/tasks/2-control-flow/) - revision for loops and conditionals

**Tutorial**

- [Tutorial 3.2]({{ site.baseurl }}/tutorials/3-2/) - guided project for this unit
