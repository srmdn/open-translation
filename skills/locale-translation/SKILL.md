---
name: locale-translation
description: Use this for app localization files and UI strings, including JSON, YAML, JS, or TS locale dictionaries. Preserves keys, placeholders, tags, and other runtime-sensitive tokens while producing concise natural UI text.
---

# Locale Translation

Translate locale values safely.

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

Prefer:

- `Saat Anda mengeklik ...`
- `"Tambah Refleksi" akan membuka ...`
- `Karusel kartu flash` if the product localizes `carousel`

Over:

- `Mengeklik ... akan ...`
- long explanatory UI labels
- literal carryover of interface nouns without checking product style

## Final Check

- Are all keys unchanged?
- Are placeholders and tags preserved?
- Is the resulting file still valid?
- Does the UI text sound like product copy, not translated prose?
