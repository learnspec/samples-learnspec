---
title: Conditions
lang: en
estimated_time: 30min
tags: [python, conditions, if-else]
---

### Lesson 1 — The `if` statement

An `if` statement runs code only when a condition evaluates to `True`.

```python
age = 20

if age >= 18:
    print("You are an adult")
```

> [!important]
> Python uses **indentation** (4 spaces) to define code blocks — not braces `{}`.

### Lesson 2 — `if` / `else`

The `else` clause runs when the condition is `False`:

```python
temperature = 35

if temperature > 30:
    print("It's hot!")
else:
    print("It's comfortable.")
```

### Lesson 3 — `elif` chains

Use `elif` to test multiple conditions in sequence:

```python
score = 75

if score >= 90:
    grade = "A"
elif score >= 80:
    grade = "B"
elif score >= 70:
    grade = "C"
else:
    grade = "F"

print(grade)  # C
```

> [!tip]
> Python evaluates conditions top to bottom and stops at the first match. Order matters!

### Lesson 4 — Comparison and logical operators

| Operator | Meaning |
|----------|---------|
| `==` | Equal to |
| `!=` | Not equal to |
| `>`, `<` | Greater / less than |
| `>=`, `<=` | Greater or equal / less or equal |
| `and` | Both conditions true |
| `or` | At least one condition true |
| `not` | Negates a condition |

```python
age = 25
has_license = True

if age >= 18 and has_license:
    print("You can drive")
```

```summary
- `if` executes a block when its condition is `True`
- `else` handles the opposite case
- `elif` chains test multiple conditions in order
- Logical operators (`and`, `or`, `not`) combine conditions
- Indentation defines code blocks in Python
```
