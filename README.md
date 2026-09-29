# DevHTMLNoteMaker

> **KnowledgeForge** — turn raw course material into **lean, interview-ready study notes** for **coding & software-development** topics (primarily .NET / ASP.NET Core backend).

KnowledgeForge **edits** your material rather than transcribing it. It keeps only what a backend interviewer would ask or a real job would use. It adds the real-world layer courses skip: deployment, API behaviour, testing, troubleshooting and design judgement. Then it connects the topic to the rest of the subject.

---

## What it produces

Every note is **two files**:

| File | What's inside |
|---|---|
| **`.md`** — the source of truth | Core idea → topic sections ordered by real usage → best practices → troubleshooting checklist → quick reference + "facts to memorize" → 10–15 concise interview Q&As. Written first, reviewed and edited by you. |
| **`.html`** — built from the reviewed `.md` | 📘 **Notes** tab: a 🧭 **mind map** linking the topic to its neighbours (fullscreen + zoom), a sticky Index sidebar with scroll-spy, highlighted code, and small flow diagrams. 💼 **Interview** tab: the Q&As as reveal cards, each linking back to its section. |

### Highlights

- **Filtered, not transcribed:** every source item must pass one test — *would an interviewer ask it, or would I use it on the job?*
- **Real-world first:** production deployment, APIs, testing and failure modes, not just the lecture demo.
- **Connected:** a mind map ties each topic to the ones it depends on.
- **Say it once:** no repeated summary layers; short prose plus code.
- **Single file, zero install:** open the `.html` anywhere; dark `Syne` + `DM Mono` theme; works offline after first load.
- **Optional extras on request:** Active Recall, Compare tables, React demos.

---

## How it works

1. **Drop material** anywhere and point KnowledgeForge at it (PDF, Markdown, text, code).
2. Say **create notes**. It reads the persona and every source, filters them, and writes the **`.md`**.
3. **Review and edit** the `.md`.
4. It builds the **`.html`** from your reviewed `.md`, faithfully, with nothing re-added.

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
