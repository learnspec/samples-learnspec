---
title: Variables and Data Types — Check
lang: en
tags: [python, variables, types]
domain: academic
shuffle_answers: true
passing_score: 0.6
reveal: sequential
feedback_mode: immediate
---

# Variables and Data Types — Check

## Q1 · Which syntax correctly creates a variable in Python?

- [x] age = 25
  > Correct — Python uses `=` for assignment, no type keyword needed.
- [ ] int age = 25
  > That's Java or C syntax, not Python.
- [ ] var age = 25
  > `var` is used in JavaScript, not Python.
- [ ] let age = 25
  > `let` is used in JavaScript, not Python.

## Q2 · What does `type(3.14)` return?

```quiz
difficulty: easy
```

- [ ] `<class 'int'>`
- [x] `<class 'float'>`
- [ ] `<class 'str'>`
- [ ] `<class 'number'>`

> `3.14` has a decimal point, so Python stores it as a `float`.

## Q3 · True or false: `Name` and `name` refer to the same variable in Python.

- [ ] True
- [x] False

> Python is case-sensitive: `Name` and `name` are two distinct variables.

## Q4 · Fill in the blank: To convert the string `"42"` to an integer, use ___.

```quiz
difficulty: easy
```

**Answer:** int("42")

> The `int()` function converts a string of digits to an integer.

## Q5 · Which of the following are valid Python data types?

```quiz
type: multi
points: 2
```

- [x] int
- [x] str
- [ ] char
- [x] bool
- [ ] double
- [x] float

> Python has `int`, `float`, `str`, and `bool`. There is no `char` or `double` type — Python uses `str` for single characters and `float` for all decimals.
