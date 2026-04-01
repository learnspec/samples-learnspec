---
title: Web Development Fundamentals — Quiz
lang: en
tags: [web, html, css]
domain: academic
passing_score: 0.6
shuffle_answers: true
reveal: all
feedback_mode: immediate
scoring:
  correct: 2
  incorrect: 0
---

# Web Development Fundamentals — Quiz

## Q1 · What does HTML stand for?

```quiz
difficulty: easy
```

- [x] HyperText Markup Language
- [ ] High-Tech Modern Language
- [ ] HyperText Making Language
- [ ] Home Tool Markup Language

> HTML stands for HyperText Markup Language — the standard language for structuring web content.

## Q2 · Which HTML element is used for the largest heading?

- [x] `<h1>`
- [ ] `<h6>`
- [ ] `<heading>`
- [ ] `<title>`

> `<h1>` is the largest heading. Headings go from `<h1>` (most important) to `<h6>` (least important).

## Q3 · What is the recommended way to add CSS to a web page?

- [ ] Inline styles
- [ ] Internal `<style>` block
- [x] External stylesheet via `<link>`
- [ ] JavaScript injection

> External stylesheets keep HTML and CSS separated and allow styles to be reused across multiple pages.

## Q4 · True or false: The `alt` attribute on `<img>` is optional and has no impact on accessibility.

- [ ] True
- [x] False

> The `alt` attribute is essential for accessibility. Screen readers use it to describe images to visually impaired users, and it displays as fallback text when images fail to load.

## Q5 · Match each CSS selector type with its syntax.

```quiz
type: match
points: 3
difficulty: easy
```

| Selector type | Syntax |
|--------------|--------|
| Element | h1 |
| Class | .highlight |
| ID | #main-title |

## Q6 · Which of the following are layers of the CSS box model?

```quiz
type: multi
points: 2
difficulty: medium
```

- [x] Content
- [x] Padding
- [x] Border
- [x] Margin
- [ ] Shadow
- [ ] Outline

> The four layers of the box model are content, padding, border, and margin. Shadow and outline exist as CSS properties but are not part of the box model.

## Q7 · Fill in the blank: To include padding and border in an element's total width, use ___.

```quiz
difficulty: medium
```

**Answer:** box-sizing: border-box

> `box-sizing: border-box` makes the width property include content, padding, and border — simplifying layout calculations.

## Q8 · Which HTML elements are considered semantic?

```quiz
type: multi
points: 2
difficulty: medium
```

- [x] `<article>`
- [x] `<nav>`
- [ ] `<div>`
- [x] `<footer>`
- [ ] `<span>`
- [x] `<header>`

> `<div>` and `<span>` are generic containers with no semantic meaning. `<article>`, `<nav>`, `<footer>`, and `<header>` describe their content's purpose.
