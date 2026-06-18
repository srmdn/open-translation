---
name: general-translation
description: Use this for general translation between languages when the goal is natural, human-sounding output rather than domain-specific formatting rules. Best for prose, chat, essays, articles, and everyday text. Supports source and target language as runtime parameters.
---

# General Translation

Translate for meaning, tone, and readability.

## Use Cases

- prose
- chat
- articles
- notes
- essays
- general rewriting across languages

## Core Rules

- Prioritize meaning over literal wording.
- Preserve tone, emphasis, and intent.
- Keep names, brands, URLs, code identifiers, and placeholders unchanged unless the user asks otherwise.
- Do not add claims, examples, or opinions.
- Make the output sound like native writing in the target language.
- Prefer natural target-language flow over grammatically faithful but flat sentence structure.

## Inputs To Infer

- source language
- target language
- tone
- audience

## Output Standard

- natural, not word-for-word
- faithful, not embellished
- readable, not stiff

## Wording Guidance

- Replace stiff procedural openers with more natural sentence flow when meaning stays intact.
- Avoid generic product nouns if the target language has a simpler, more human phrasing.
- Rewrite abstract explanatory prose so it reads like something a person would naturally say or write.

Prefer:

- `Saat Anda mengeklik ...`
- `tempat untuk berbagi ...`
- direct, flowing sentence structure

Over:

- `Mengeklik ... akan ...`
- `platform untuk ...` when it adds no value
- accurate but flat sentence structure

## Final Check

- Does it sound written by a native speaker?
- Was any meaning lost or exaggerated?
- Are fixed tokens preserved?
- Is the sentence flow natural, not just correct?
