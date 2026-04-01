---
title: Variables and Data Types
lang: en
estimated_time: 30min
tags: [python, variables, types]
---

### Lesson 1 — What is a variable?

A variable is a named reference to a value stored in memory. In Python, you create a variable by assigning a value with `=`.

```python
age = 25
name = "Alice"
pi = 3.14
```

> [!tip]
> Use descriptive names: `student_count` is clearer than `n`.

> [!warning]
> Variable names are case-sensitive: `Age` and `age` are two different variables.

### Lesson 2 — Basic data types

Python infers types automatically — no type declarations needed.

| Type | Example | Description |
|------|---------|-------------|
| `int` | `42` | Whole numbers |
| `float` | `3.14` | Decimal numbers |
| `str` | `"hello"` | Text strings |
| `bool` | `True` | Boolean values |

```python
age = 25         # int
pi = 3.14        # float
name = "Alice"   # str
active = True    # bool
```

You can inspect a value's type with the built-in `type()` function:

```python
print(type(25))       # <class 'int'>
print(type(3.14))     # <class 'float'>
print(type("hello"))  # <class 'str'>
print(type(True))     # <class 'bool'>
```

### Lesson 3 — Type conversion

Python provides built-in functions to convert between types:

```python
# String to integer
num = int("42")       # 42

# Integer to string
text = str(100)       # "100"

# Integer to float
decimal = float(7)    # 7.0
```

> [!warning]
> Converting an invalid string raises an error:
> `int("hello")` → `ValueError`

```summary
- Variables associate a **name** with a **value**
- Python infers types dynamically — no declaration needed
- Four basic types: `int`, `float`, `str`, `bool`
- Use `type()` to inspect, and `int()`, `str()`, `float()` to convert
- Names are case-sensitive: `Age` ≠ `age`
```
