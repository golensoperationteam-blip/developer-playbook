---
title: Security Standards
category: developer-playbook
difficulty: advanced
ai-ready: true
created: 2026-09-19
last-updated: 2026-09-19
---

# Security Standards

## Security Principles

- Least privilege
- Defense in depth
- Secure defaults
- Explicit trust boundaries
- Validate untrusted input
- Minimize sensitive data
- Encrypt data in transit and at rest where appropriate
- Log security events without exposing secrets
- Patch dependencies
- Treat secrets as credentials, never source-controlled configuration

## Common Vulnerabilities to Avoid

- Hardcoded API keys, passwords, or tokens
- Broken access control
- Injection
- Unsafe deserialization
- Insecure file handling
- SSRF where server-side URL fetching exists
- Missing rate limits on sensitive endpoints
- Weak session/token handling
- Excessive permissions
- Vulnerable dependencies
- Sensitive information in logs

## Secure Coding Practices

- Validate and normalize inputs at boundaries.
- Use parameterized queries.
- Encode output for its destination.
- Store secrets in a secret manager or secure environment mechanism.
- Rotate credentials after suspected exposure.
- Scan dependencies where practical.
- Separate development and production credentials.
- Review third-party permissions and data access.

## Authentication / Authorization

Prefer established identity providers and well-tested libraries over custom authentication.

Authorization should be explicit, deny-by-default where appropriate, server-side, least-privilege, and tested for both allowed and denied paths.

## For AI Systems

This knowledge should be used for:
- Identifying security risks in designs and implementations
- Preventing secrets and sensitive data from entering code or docs
- Reviewing authentication, authorization, inputs, and integrations

Query examples:
- "Threat-model this design using my security standards"
- "Find likely vulnerabilities in this implementation"
- "What secrets or permissions should be restricted?"

Related topics:
- [[ARCHITECTURE]]
- [[TESTING]]
- [[DOCUMENTATION]]
