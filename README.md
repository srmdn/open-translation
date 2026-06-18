# open-translation

Open translation skills and tooling for humans, AI agents, and developers.

Initial quality target:

- English <-> Indonesian

The goal is not generic machine translation. The goal is translation that is:

- natural
- human-sounding
- structurally safe when format matters
- reusable across agent workflows and future tooling

## Current Scope

This repo currently focuses on task-based translation skills.

Available public skills:

- `general-translation`
- `technical-docs-translation`
- `locale-translation`
- `marketing-translation`
- `subtitle-translation`
- `religious-content-translation`
- `anti-slop-writing`
- `translation-review`

The project is organized by task type, not by language-pair folder explosion.

That means the intended model is:

- task type as the main skill boundary
- source language and target language as runtime inputs

## Principles

- keep each skill focused
- prefer composition over one large mixed-purpose skill
- preserve meaning and tone
- avoid AI-sounding filler and stiffness
- keep code, Markdown, locale tokens, and other runtime-sensitive structure safe
- use evaluation to refine skills, not only intuition

## Repo Layout

```text
skills/
  <skill-name>/
    SKILL.md
AGENTS.md
CONTRIBUTING.md
LICENSE
```

Local/private planning and evaluation may exist under `.local/`, but that workspace is optional and not part of the public repo contract.

## Status

Current state:

- initial skill set scaffolded
- private PRD and roadmap in local workspace
- private evaluation harness seeded with real OSS translation cases
- first evaluation-driven refinements already applied to docs and locale skills

Planned later:

- MCP surface
- web surface
- broader language coverage

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md).

Short version:

- keep edits narrow
- avoid duplicating guidance across skills
- preserve clear scope boundaries
- optimize for human-sounding output, not generic prompt bloat

## License

[Apache-2.0](./LICENSE)
