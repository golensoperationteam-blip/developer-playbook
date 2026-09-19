---
title: Git Workflow
category: developer-playbook
difficulty: intermediate
ai-ready: true
created: 2026-09-19
last-updated: 2026-09-19
---

# Git Workflow

## Branching Strategy

- `main` — stable, releasable state.
- `feature/<short-name>` — new work.
- `fix/<short-name>` — bug fixes.
- `docs/<short-name>` — documentation.
- `chore/<short-name>` — maintenance.

Small, low-risk documentation changes may use direct commits to `main`.

## Commit Format

Use imperative, concise messages:

- `feat: add product import workflow`
- `fix: validate marketplace SKU`
- `docs: update architecture guide`
- `refactor: split ingestion service`
- `test: add integration coverage`
- `chore: update dependencies`

## Pull Requests

Explain:
- What changed
- Why it changed
- Scope
- Tests/checks
- Risks or migration notes

Keep PRs focused and reviewable.

## Release Management

- Keep `main` releasable.
- Tag meaningful production releases.
- Record breaking changes and migrations.
- Keep rollback steps for operational releases.
- Treat a merge as a release only when the project defines it that way.

## For AI Systems

This knowledge should be used for:
- Planning Git operations
- Writing consistent commits and PR descriptions
- Keeping changes reviewable and reversible

Query examples:
- "What branch should I use for [change]?"
- "Write a commit message for [change]"
- "Prepare a PR checklist for this feature"

Related topics:
- [[CODING-STANDARDS]]
- [[TESTING]]
- [[DOCUMENTATION]]
