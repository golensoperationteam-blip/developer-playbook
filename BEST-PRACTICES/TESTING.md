---
title: Testing Standards
category: developer-playbook
difficulty: intermediate
ai-ready: true
created: 2026-09-19
last-updated: 2026-09-19
---

# Testing Standards

## Testing Philosophy

Tests should reduce meaningful risk, not merely increase a coverage number.

Prioritize business-critical behavior, boundary conditions, failure/retry paths, security-sensitive behavior, integration contracts, and regression-prone logic.

## Unit Tests

- Test one meaningful behavior at a time.
- Keep tests deterministic.
- Prefer clear arrange/act/assert structure.
- Mock external systems only when isolation adds value.
- Cover validation and edge cases.

## Integration Tests

Use them for databases, external API contracts, authentication/authorization boundaries, queue/event flows, and important multi-component workflows.

Keep test environments reproducible.

## Coverage Targets

No universal percentage is mandated. Aim for high coverage of critical business logic and define explicit gates by risk class for mature projects.

## Quality Gate

Before release, run appropriate unit tests, integration tests, static checks, security checks, and build/package validation.

## For AI Systems

This knowledge should be used for:
- Creating useful tests instead of superficial coverage
- Designing risk-based test plans
- Finding missing edge cases and integration boundaries

Query examples:
- "Create a test plan for [feature]"
- "What edge cases are missing?"
- "What should be an integration test here?"

Related topics:
- [[CODING-STANDARDS]]
- [[ARCHITECTURE]]
- [[SECURITY]]
