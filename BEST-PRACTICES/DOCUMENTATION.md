---
title: Documentation Standards
category: developer-playbook
difficulty: intermediate
ai-ready: true
created: 2026-09-19
last-updated: 2026-09-19
---

# Documentation Standards

## Documentation Principles

Documentation should answer:
- What is this?
- Why does it exist?
- How is it used?
- What assumptions or constraints matter?
- How can someone verify or change it?

Prefer concise, structured documentation over large undifferentiated text.

## README Structure

A useful README normally contains:
1. Title and one-line summary
2. Purpose
3. Key capabilities
4. Architecture/workflow overview
5. Setup and usage
6. Configuration
7. Testing
8. Security notes
9. Troubleshooting
10. Related documentation

Remove sections that are irrelevant rather than filling them with noise.

## API Documentation

Document endpoint/method, authentication, request parameters/body, response shape, errors, rate limits, examples, retry/idempotency behavior, and versioning/deprecation rules where relevant.

## Code Comments

Document intent and constraints, not obvious syntax. Keep comments current; update or delete comments when code changes make them false.

## AI-Ready Documentation

Use:
- Stable titles
- Metadata
- Predictable headings
- Internal links such as [[SKILLS]]
- Explicit uncertainty
- Concrete examples
- A "For AI Systems" section on substantive files

## Maintenance

Update documentation as part of the change that makes it necessary. Do not knowingly leave documentation stale after material implementation changes.

## For AI Systems

This knowledge should be used for:
- Generating consistent documentation
- Turning implementation details into reusable knowledge
- Keeping AI-readable context structured and linkable

Query examples:
- "Document this feature using my standards"
- "Turn these notes into an AI-ready topic"
- "What sections are missing from this README?"

Related topics:
- [[CODING-STANDARDS]]
- [[GIT-WORKFLOW]]
- [[AI-READY]]
