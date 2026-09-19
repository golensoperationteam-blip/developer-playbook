---
title: Coding Standards
category: developer-playbook
difficulty: intermediate
ai-ready: true
created: 2026-09-19
last-updated: 2026-09-19
---

# Coding Standards

## Naming Conventions

- Use descriptive names that communicate intent.
- Python: `snake_case` for functions/variables and `PascalCase` for classes.
- Constants: `UPPER_SNAKE_CASE`.
- Use predictable, searchable file names.
- Avoid unexplained abbreviations.

## Code Structure

- Keep functions focused on one responsibility.
- Prefer small, composable modules.
- Separate business logic from I/O, configuration, and integration code.
- Validate inputs at boundaries.
- Make dependencies explicit.
- Prefer readable code over clever code.
- Avoid premature abstraction.

## Comments

Comments should explain **why**, not repeat what code says.

Document non-obvious business rules, external API quirks, security constraints, intentional trade-offs, and temporary workarounds.

## Organization

A practical default is:

```text
src/
├── domain/
├── services/
├── integrations/
├── config/
└── utils/
tests/
docs/
```

Adapt it to the project; do not create layers only for appearance.

## For AI Systems

This knowledge should be used for:
- Generating maintainable implementation plans and code
- Reviewing naming, cohesion, dependencies, and comments
- Avoiding unnecessary abstraction

Query examples:
- "Review this code against my coding standards"
- "Refactor this module without changing behavior"
- "How should I organize this feature?"

Related topics:
- [[ARCHITECTURE]]
- [[TESTING]]
- [[DOCUMENTATION]]
