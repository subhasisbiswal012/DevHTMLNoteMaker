# DevHTMLNoteMaker

> **KnowledgeForge** — turn raw study material into a single, self-contained, interactive HTML note built for deep understanding and long-term retention of **coding & software-development** topics.

Drop your material in, get back one `.html` file you can open in any browser — no build step, no server, no dependencies to install. It bundles a visual handbook, active-recall questions, real interview questions, and topic comparisons into one file.

---

## What it produces

Every note is **one self-contained `.html` file** with four tabs and a sticky Index:

| Tab | What's inside |
|---|---|
| 📘 **Handbook** | Example-first explanations, inline SVG diagrams, syntax-highlighted code, Wrong-vs-Right panels, and a sticky **Index sidebar** with scroll-spy navigation. |
| 🧠 **Active Recall** | Retrieval questions (`DEF` / `APPLY` / `WHY` / `COMPARE` / `SEQUENCE` / `GOTCHA` / `DRAW`) with per-question show/hide answers and a live progress counter. |
| 💼 **Interview** | Real interview-grade questions tagged `Junior` / `Mid` / `Senior`, each with **"what they're really testing"** and likely follow-ups. |
| ⚖️ **Compare** | Topic-level comparisons: concept-vs-concept tables, "when to use what" decision guides, trade-off cards, and old-way→new-way evolution. |

### Highlights

- **Single file, zero install** — open the `.html` anywhere; works offline after first load.
- **Dark, focused design** — custom theme, `Syne` + `DM Mono` fonts, grid texture.
- **Real diagrams, never ASCII** — flowcharts, pipelines, trees, request/response, nesting models as inline SVG.
- **React only when it earns it** — interactive demos and simulators load React via CDN *only* when hands-on beats a static diagram; otherwise notes stay lightweight vanilla JS.
- **Subtle motion by default**, richer animation on request, with `prefers-reduced-motion` respected.
- **📎 Worth-knowing additions** — must-know essentials beyond your source, always clearly marked.

---

## How it works

1. **Drop material** into your `Notes material/` folder (PDF, Markdown, text, code, links).
2. Tell KnowledgeForge to **create notes** for the topic.
3. It reads the persona, reads your material, and writes a `[Topic-Name]-KnowledgeForge.html` into your `HTML Notes/` folder.
4. Open the file in a browser. Study, recall, prep, compare.

The full behaviour is defined in [`persona.md`](./persona.md) — the KnowledgeForge system prompt. Point your Claude project at it.

> **Note:** This repository contains the **note-maker system only** (the persona, license, and docs). Your own study material (inputs) and generated notes (outputs) stay local and are never published.

---

## Tech

- HTML + CSS + vanilla JavaScript, single self-contained file
- [highlight.js](https://highlightjs.org/) for syntax highlighting (CDN)
- [Google Fonts](https://fonts.google.com/) — Syne + DM Mono (CDN)
- [React](https://react.dev/) + Babel Standalone (CDN) — loaded only for interactive demos

---

## Contributing

This repo is **open to contributions** — got an idea to make the notes better (new diagram types, tab features, question styles, theme options)? Open an issue or a PR. Improvements to the `persona.md` rules are especially welcome.

---

## License

[MIT](./LICENSE) © 2026 Subhasis Biswal

---

## Author

**Subhasis Biswal**

- GitHub — https://github.com/subhasisbiswal012
- YouTube — https://www.youtube.com/@avidyant
- LinkedIn — https://www.linkedin.com/in/subhasis-biswal-593851157/
