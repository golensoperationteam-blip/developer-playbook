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

## Verified Git Workflow Practice

This section records the repository workflow verified through a guided feature-branch and pull-request exercise.

### Feature Branch Creation

1. Start from an up-to-date `main` branch.
2. Create a focused branch using the repository naming convention, such as `feature/<short-name>`.
3. Confirm the branch points to the intended `main` baseline before making changes.

### Focused Changes

- Keep the change limited to one clearly defined objective.
- Modify only the documentation file required for that objective.
- Inspect the working diff before committing to catch unrelated changes.

### Commit Conventions

- Use an imperative, concise Conventional Commit-style message.
- Make one logical change per commit when practical.
- For this verification exercise, the commit message is:
  `docs: document verified git workflow practice`

### Pull Request Review

Before merging, inspect the pull request diff and verify:

- Only intended files changed.
- Markdown formatting is valid and readable.
- No secrets or credentials are present.
- Internal links remain valid.
- Content is consistent with repository standards.

### Merge Verification

After an approved merge:

1. Confirm the pull request is merged into `main`.
2. Record the merge commit SHA when GitHub provides one.
3. Verify the changed content exists on `main`.
4. Confirm no unrelated files were introduced by the merge.

This workflow provides a repeatable, reviewable path from a focused feature branch to verified documentation on `main`.

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
