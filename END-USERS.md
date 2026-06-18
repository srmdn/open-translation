# End Users

`open-translation` is intended to become a translation toolset for humans and AI users who want output that sounds natural, preserves meaning, and stays structurally safe when format matters.

## What To Expect

The project is optimized for:

- human-sounding translation
- better handling of structure-sensitive content such as locale strings and technical docs
- task-based behavior instead of one generic translation mode

Current task types include:

- general translation
- technical docs translation
- locale translation
- marketing translation
- subtitle translation
- religious content translation
- anti-slop rewriting
- translation review

## Quality Expectations

The goal is not just correctness. The goal is output that is:

- faithful to the source
- natural in the target language
- structurally safe when tokens, markup, or code matter

## Limitations

Quality can still vary depending on:

- the task type
- the source and target language direction
- terminology policy for the domain
- the model or runtime behind the tool

For sensitive or terminology-heavy content, review may still be useful even when the output is already strong.

## Current Project State

The repo is still focused on skill design and evaluation rather than a polished end-user product.

Planned later:

- MCP tools
- web interface
- broader language coverage
