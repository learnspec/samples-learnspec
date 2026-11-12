# samples-learnspec

Sample content written in [LearnMD](https://github.com/learnspec/learnmd) and [QuizMD](https://github.com/learnspec/quizmd) — open formats for structured learning in the AI era.

## Samples

| Folder | Topic | Features showcased |
|--------|-------|--------------------|
| [`python-basics/`](python-basics/) | Introduction to Python | Multi-file path with `!import`, inline `quiz` checkpoints, fenced `summary` and `example` blocks |
| [`solar-system/`](solar-system/) | Our Solar System | LaTeX math ($F = G \frac{m_1 m_2}{r^2}$), `match` and `order` question types, GFM callouts |
| [`music-theory/`](music-theory/) | Music Theory Fundamentals | ABC music notation with `play`/`cursor` flags, `match` and `order` questions |
| [`web-fundamentals/`](web-fundamentals/) | Web Development Fundamentals | Code blocks (HTML, CSS), `multi` question type, scored inline quizzes |
| [`water-cycle/`](water-cycle/) | The water cycle | [AnimMD](https://github.com/learnspec/animmd) step-reveal animation over a [DiagramMD](https://github.com/learnspec/diagrammd) stock entry, referenced animated and static from the same lesson |

## Format overview

- **LearnMD** (`.learn.md`) — Markdown-based format for instructional content: lessons, modules, examples, and embedded quiz checkpoints.
- **QuizMD** (`.quiz.md`) — Markdown-based format for assessments: MCQ, multi-select, true/false, open answer, match pairs, and ordering questions.

Both formats are:
- **Markdown-first** — readable in any editor or on GitHub
- **Git-native** — versionable, diffable, mergeable
- **AI-native** — generatable and consumable by LLMs
- **Progressively enriched** — plain text up through rich interactive blocks

## Getting started

1. Browse the samples on GitHub — they render as readable Markdown.
2. Use the [memoneo MCP server](https://memoneo.app) to parse, validate, and publish content.
3. Write your own `.learn.md` and `.quiz.md` files following the specs:
   - [LearnMD spec](https://github.com/learnspec/learnmd)
   - [QuizMD spec](https://github.com/learnspec/quizmd)

## Maintainers

This repository is part of the [LearnSpec](https://learnspec.org) suite, initiated and maintained by [memoneo](https://memoneo.app). Issues and pull requests are welcome.

## License

CC-BY-4.0
