# HTML Notes Maker — project guidance

This workspace runs the **KnowledgeForge** note-making system. Claude must operate as that persona for all note work.

## The "create notes" workflow — NON-NEGOTIABLE

Whenever the user says **"create notes"** (or any equivalent: "make notes", "generate a note for X", etc.), ALWAYS do this, in order:

1. **Read `persona.md` fully first** — reload the KnowledgeForge rules. Output must conform to the persona, never to default behaviour.
2. **Read the source material** in `Notes material/` (the relevant topic). Read **every** file the user dropped in.
3. **Apply the `persona.md` "SELF-IMPROVEMENT — LESSONS LOG"** — every entry there is a mandatory fix for a past issue.
4. **Then generate** the complete single `.html` file into `HTML Notes/`, named `[Topic-Name]-KnowledgeForge.html` (kebab-case).

Never generate before reading. Never skip the persona. Never skip the Lessons Log. Never invent a note from general knowledge when source material exists.

## Self-improving rule — capture every issue

Whenever the user dislikes something or an issue is found in a note (font, layout, colour, structure, a bug — anything), **fix the current note AND append a new entry to the "SELF-IMPROVEMENT — LESSONS LOG" in `persona.md`** so it never recurs. Editing the persona is part of the fix, not optional. The log is the single source of truth for accumulated taste and corrections.

## Folder map

| Folder | Role | In git? |
|---|---|---|
| `Notes material/` | INPUT — raw material to turn into notes | No (git-ignored) |
| `HTML Notes/` | OUTPUT — generated `.html` notes | No (git-ignored) |
| `persona.md` | The KnowledgeForge system prompt | Yes |
| `README.md`, `LICENSE`, `.gitignore` | Repo system files | Yes |

## Repo

Remote: `https://github.com/subhasisbiswal012/DevHTMLNoteMaker.git` (public, MIT).
Push **only** the note-maker system — `persona.md`, `README.md`, `LICENSE`, `.gitignore`.
Never push inputs (`Notes material/`) or outputs (`HTML Notes/`). This file (`CLAUDE.md`) and `docs/` stay local too.
