---
title: Loops
lang: en
estimated_time: 30min
tags: [python, loops, for, while]
---

### Lesson 1 — The `for` loop

A `for` loop iterates over a sequence (list, string, range, etc.):

```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
```

Output:

```
apple
banana
cherry
```

### Lesson 2 — The `range()` function

`range()` generates a sequence of numbers — commonly used with `for`:

```python
for i in range(5):
    print(i)  # prints 0, 1, 2, 3, 4
```

> [!note]
> `range(5)` produces numbers from `0` to `4` (the stop value is exclusive).

You can also specify start and step:

```python
for i in range(2, 10, 2):
    print(i)  # prints 2, 4, 6, 8
```

### Lesson 3 — The `while` loop

A `while` loop repeats as long as its condition is `True`:

```python
count = 0

while count < 3:
    print(count)
    count += 1
```

> [!warning]
> Forgetting to update the loop variable causes an **infinite loop**. Always ensure the condition will eventually become `False`.

### Lesson 4 — `break` and `continue`

- `break` exits the loop immediately
- `continue` skips to the next iteration

```example python title:"Finding the first even number"
numbers = [1, 3, 4, 7, 8]

for n in numbers:
    if n % 2 == 0:
        print(f"First even: {n}")
        break
# Output: First even: 4
```

```example python title:"Skipping odd numbers"
for n in range(6):
    if n % 2 != 0:
        continue
    print(n)
# Output: 0, 2, 4
```

```summary
- `for` iterates over sequences (lists, strings, ranges)
- `range(n)` generates numbers from `0` to `n-1`
- `while` repeats as long as its condition is `True`
- `break` exits a loop early; `continue` skips to the next iteration
- Always ensure `while` loops can terminate
```
