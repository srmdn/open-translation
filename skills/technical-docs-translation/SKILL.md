---
name: technical-docs-translation
description: Use this for translation or review of technical documentation, README files, Markdown, MDX, tutorials, and developer guides. Preserves code-sensitive structure while keeping the prose natural in the target language.
---

# Technical Docs Translation

Translate developer documentation without breaking code, structure, or terminology.

## Scope Boundary

- Use this for developer-facing docs where Markdown, MDX, code samples, commands, or framework terms matter.
- For general prose without code-sensitive structure, use `general-translation`.
- For app locale files or UI dictionaries, use `locale-translation`.

## Use Cases

- README
- Markdown
- MDX
- framework docs
- API guides
- tutorials
- developer references

## Core Rules

- Translate prose, not executable code.
- Preserve code fences, inline code, commands, paths, imports, exports, URLs, placeholders, JSX/component names, and frontmatter keys.
- Translate frontmatter values only when they are human-facing text.
- Keep common developer terms in the source language when translating them would slow comprehension.
- Keep technical terminology consistent within the file.
- Avoid stacking too many English words into one untranslated phrase when the surrounding prose can be localized more naturally.
- If project-visible labels such as admonition tags or heading conventions are ambiguous, follow the file's existing convention instead of localizing inconsistently.

## Typical Inputs

- source language
- target language
- format such as `markdown` or `mdx`
- domain such as framework docs or API docs

## Failure Modes To Prevent

- broken Markdown or MDX
- translated code identifiers
- literal phrasing around technical concepts
- inconsistent terminology
- mixed-language prose that sounds imported rather than written naturally

## Wording Guidance

- Keep developer terms in English when needed, but localize the surrounding phrase naturally.
- Do not preserve an English phrase mechanically just because one term inside it should remain English.
- Avoid literal carryover such as `membuat scaffold` when a more natural phrase is available.
- Reduce mixed-language phrase stacking when a short Indonesian frame keeps the developer meaning just as clear.
- When a conceptual phrase sounds literal after translation, rewrite the surrounding sentence so it matches how developers actually describe the idea in the target language.

Prefer:

- `editor teks dengan dukungan sintaks Markdown`
- `setup wizard di command line`
- `menyiapkan struktur awal proyek`
- `wizard setup berbasis command line`
- `struktur data yang konsisten`

Over:

- `Text Editor dengan dukungan sintaks Markdown`
- `command line setup wizard`
- `membuat scaffold proyek`
- `bentuk yang konsisten`

## Final Check

- Is the structure intact?
- Is the prose natural for developers in the target language?
- Were code-sensitive regions preserved exactly?
- Are English technical terms used intentionally rather than piled together awkwardly in prose?
