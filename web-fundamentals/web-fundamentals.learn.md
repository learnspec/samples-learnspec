---
title: Web Development Fundamentals
lang: en
estimated_time: 1h30
tags: [web, html, css, beginner]
author: learnspec
---

# Web Development Fundamentals

Learn the core technologies that power every website — HTML for structure, CSS for style.

> [!objectives]
> After this lesson, you will be able to:
> - Write a valid HTML page with headings, paragraphs, links, and images
> - Apply CSS styles to control colours, fonts, and layout
> - Understand the box model and how elements are sized

## Module 1 — HTML Basics

### Lesson 1 — Your first HTML page

HTML (HyperText Markup Language) uses **tags** to structure content. Every HTML page has the same skeleton:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My First Page</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>This is my first web page.</p>
</body>
</html>
```

> [!important]
> Every HTML document must start with `<!DOCTYPE html>` to tell the browser which version of HTML to use.

### Lesson 2 — Common HTML elements

| Element | Purpose | Example |
|---------|---------|---------|
| `<h1>`–`<h6>` | Headings (1 = largest) | `<h1>Title</h1>` |
| `<p>` | Paragraph | `<p>Some text.</p>` |
| `<a>` | Hyperlink | `<a href="url">Click</a>` |
| `<img>` | Image | `<img src="photo.jpg" alt="desc">` |
| `<ul>`, `<ol>` | Lists | `<ul><li>Item</li></ul>` |
| `<div>` | Generic container | `<div>...</div>` |

> [!tip]
> Always include the `alt` attribute on `<img>` tags — it improves accessibility for screen readers and is displayed when the image fails to load.

```quiz
? Which tag creates the largest heading?
- [x] `<h1>`
- [ ] `<h6>`
- [ ] `<header>`
- [ ] `<title>`
```

### Lesson 3 — Semantic HTML

Semantic elements describe their content's meaning, making pages more accessible and SEO-friendly:

```html
<header>
    <nav>
        <a href="/">Home</a>
        <a href="/about">About</a>
    </nav>
</header>

<main>
    <article>
        <h2>Article Title</h2>
        <p>Article content...</p>
    </article>
</main>

<footer>
    <p>&copy; 2025 My Website</p>
</footer>
```

> [!note]
> Prefer `<article>`, `<section>`, `<nav>`, `<header>`, and `<footer>` over generic `<div>` tags when the content has clear meaning.

## Module 2 — CSS Fundamentals

### Lesson 4 — Adding CSS

CSS (Cascading Style Sheets) controls how HTML elements look. There are three ways to add CSS:

1. **Inline** — directly on an element (avoid for maintainability):
   ```html
   <p style="color: blue;">Blue text</p>
   ```

2. **Internal** — in a `<style>` block inside `<head>`:
   ```html
   <style>
       p { color: blue; }
   </style>
   ```

3. **External** — in a separate `.css` file (recommended):
   ```html
   <link rel="stylesheet" href="styles.css">
   ```

> [!tip]
> External stylesheets are the standard approach. They keep HTML and CSS separated and allow styles to be reused across pages.

### Lesson 5 — Selectors and properties

CSS rules consist of a **selector** and a set of **declarations**:

```css
/* selector { property: value; } */
h1 {
    color: #2c3e50;
    font-size: 2rem;
    margin-bottom: 1rem;
}

.highlight {
    background-color: yellow;
    padding: 0.25rem 0.5rem;
}

#main-title {
    text-align: center;
}
```

| Selector type | Syntax | Matches |
|--------------|--------|---------|
| Element | `h1` | All `<h1>` elements |
| Class | `.highlight` | Elements with `class="highlight"` |
| ID | `#main-title` | The element with `id="main-title"` |

### Lesson 6 — The box model

Every HTML element is a rectangular box with four layers:

```
┌─────────────────────────────────┐
│           margin                │
│  ┌───────────────────────────┐  │
│  │        border             │  │
│  │  ┌───────────────────┐    │  │
│  │  │     padding        │   │  │
│  │  │  ┌─────────────┐  │   │  │
│  │  │  │   content    │  │   │  │
│  │  │  └─────────────┘  │   │  │
│  │  └───────────────────┘    │  │
│  └───────────────────────────┘  │
└─────────────────────────────────┘
```

```css
.box {
    width: 200px;          /* content width */
    padding: 20px;         /* space inside the border */
    border: 2px solid #333; /* visible border */
    margin: 10px;          /* space outside the border */
}
```

> [!warning]
> By default, `width` sets only the **content** width. Padding and border are added on top. Use `box-sizing: border-box` to include padding and border in the total width.

```quiz scored:true
? What does `box-sizing: border-box` do?
- [x] Includes padding and border in the element's total width
- [ ] Removes the border from the element
- [ ] Adds a box shadow to the element
- [ ] Makes the element fill its parent container
```

```summary
- HTML structures content with tags; CSS controls presentation
- Use semantic elements (`<header>`, `<main>`, `<article>`, `<footer>`) for accessibility
- External stylesheets are the preferred way to add CSS
- Three CSS selector types: element (`h1`), class (`.name`), ID (`#name`)
- The box model: content → padding → border → margin
- Use `box-sizing: border-box` for predictable sizing
```
