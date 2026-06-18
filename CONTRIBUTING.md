# Contributing

Thanks for contributing to `open-translation`.

## Project Shape

This repo focuses on open translation skills and related tooling.

Current public surface:

- `skills/<skill-name>/SKILL.md`

Future surfaces may include `mcp/`, `web/`, or shared core modules, but contributions should follow the current repo structure unless maintainers expand it.

## What Good Contributions Look Like

- one clear improvement at a time
- concise skill instructions
- low duplication across skills
- explicit scope boundaries
- examples only when they materially improve behavior
- output quality that sounds human, not generic AI translation

## Skill Design Rules

- Keep each skill focused on one main job.
- Prefer task-type boundaries over language-pair folder explosion.
- Keep runtime-safety rules in the skills that need them.
- Put cross-cutting guidance in separate skills instead of copying it into every skill.
- Use YAML frontmatter with `name` and `description`.

## Before You Change A Skill

Check:

- does this belong in an existing skill, or is it a different failure mode?
- does this increase overlap with a sibling skill?
- is this rule public and reusable, or only local/private workflow?

## Public Vs Private Material

Public repo content:

- `AGENTS.md`
- `CONTRIBUTING.md`
- `LICENSE`
- `skills/`

Local-only content:

- `.local/`

Do not add `.local/` files to git. Contributors should not depend on local-only planning or eval notes to understand the public repo.

## Suggested Contribution Flow

1. Identify the target skill or propose a new one.
2. Keep the edit narrow.
3. Re-read sibling skills for overlap.
4. Make sure the skill still reads cleanly end to end.
5. If you are using a local eval workspace, add or update a case or run note.

## Pull Request Notes

- Explain the problem being fixed.
- Explain why the change belongs in that skill.
- Mention any overlap or terminology tradeoffs.
- Keep PRs small when possible.
