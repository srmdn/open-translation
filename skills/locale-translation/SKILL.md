---
name: locale-translation
description: Use this for app localization files and UI strings, including JSON, YAML, JS, or TS locale dictionaries. Preserves keys, placeholders, tags, and other runtime-sensitive tokens while producing concise natural UI text.
---

# Locale Translation

Translate locale values safely.

## Scope Boundary

- Use this for localization files, UI strings, labels, validation messages, and help text with runtime-sensitive tokens.
- Do not use this for long-form articles, essays, or developer documentation just because the text happens to be in JSON or YAML.
- If the task is mainly terminology-sensitive religious prose rather than interface copy, use `religious-content-translation`.

## Use Cases

- JSON locale files
- YAML locale files
- JS or TS dictionaries
- UI labels
- UI messages
- interface copy

## Core Rules

- Translate values, not keys.
- Preserve keys exactly.
- Preserve placeholders, interpolation variables, HTML tags, component tags, and format tokens exactly.
- Keep labels concise.
- Favor interface clarity over literary phrasing.
- Keep terminology consistent across related locale files.
- Prefer native-feeling UI wording over literal interface nouns when the localized term is already natural.
- When the product domain has sensitive terminology, keep approved terms consistent across the locale instead of inventing local variants per string.

## Typical Inputs

- source language
- target language
- format such as `json`, `yaml`, `js`, or `ts`
- product/domain terminology

## Failure Modes To Prevent

- changed keys
- broken placeholders
- broken tags
- overly long labels
- inconsistent terminology
- UI wording that is structurally safe but still sounds machine-translated

## Wording Guidance

- Keep help text and UI labels simple.
- For interaction phrasing, prefer direct UI language over stiff literal narration.
- Localize borrowed interface nouns when the target-language product style already has a natural equivalent.
- Prefer action labels that match what the control does, not mechanically literal translations of the source wording.
- If a product term such as `streak` or a bookmark/save verb has no settled policy, prefer the clearest natural wording and keep the choice consistent across related strings.

Prefer:

- `Saat Anda mengeklik ...`
- `"Tambah Refleksi" akan membuka ...`
- `Karusel kartu flash` if the product localizes `carousel`
- short action labels such as `Tambahkan`, `Tulis`, or `Buka` when they fit the UI pattern
- reminder phrasing such as `tinggal {{minutesLeft}} menit lagi` when it reads more naturally than a literal distance metaphor

Over:

- `Mengeklik ... akan ...`
- long explanatory UI labels
- literal carryover of interface nouns without checking product style

## Final Check

- Are all keys unchanged?
- Are placeholders and tags preserved?
- Is the resulting file still valid?
- Are domain terms consistent across related strings?
- Does the UI text sound like product copy, not translated prose?
