# CLAUDE.md

Instructions for Claude Code when working in this repository.

## Commit Convention

This repository follows [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<optional scope>): <short summary>
```

Allowed types:

- `feat`: a new skill, feature, or capability
- `fix`: correcting an error in an existing skill or file
- `docs`: documentation-only changes (README, CLAUDE.md, etc.)
- `refactor`: restructuring content or files without changing behavior
- `chore`: maintenance tasks (version bumps, tooling, config)

Scope, when used, matches the affected area (e.g. `feat(company): ...`, `feat(companies): ...`).

Rules:

- Summary is written in the imperative mood, lowercase, no trailing period.
- Keep the summary concise; put any further explanation in the commit body.
- See `git log` for examples of this convention in practice.

## Skill Authoring

For creating or editing Skills in this repository, follow [skill-writer/SKILL.md](skill-writer/SKILL.md).
