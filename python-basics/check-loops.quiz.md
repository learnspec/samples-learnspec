---
title: Loops — Check
lang: en
tags: [python, loops]
domain: academic
shuffle_answers: true
passing_score: 0.6
reveal: sequential
feedback_mode: immediate
---

# Loops — Check

## Q1 · What does `range(3)` produce?

- [ ] 1, 2, 3
- [x] 0, 1, 2
- [ ] 0, 1, 2, 3
- [ ] 1, 2

> `range(3)` starts at `0` and stops before `3`, producing `0, 1, 2`.

## Q2 · Which keyword exits a loop immediately?

- [x] break
- [ ] continue
- [ ] return
- [ ] stop

> `break` terminates the loop. `continue` only skips the current iteration.

## Q3 · How many times does this loop print?

```python
i = 0
while i < 5:
    print(i)
    i += 1
```

- [ ] 4
- [x] 5
- [ ] 6
- [ ] Infinite

> The loop runs for `i = 0, 1, 2, 3, 4` — five iterations.

## Q4 · Fill in the blank: To skip the current iteration and continue with the next one, use ___.

**Answer:** continue

> The `continue` statement skips the rest of the current iteration and moves to the next.

## Q5 · Place these loop events in correct execution order.

```quiz
type: order
points: 3
```

1. Check loop condition
2. Execute loop body
3. Update loop variable
4. Re-check condition
