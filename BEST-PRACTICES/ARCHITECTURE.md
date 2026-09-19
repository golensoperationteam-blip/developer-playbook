---
title: Architecture Standards
category: developer-playbook
difficulty: advanced
ai-ready: true
created: 2026-09-19
last-updated: 2026-09-19
---

# Architecture Standards

## System Design Approach

Start from requirements and constraints, not fashionable architecture.

1. Define users, inputs, outputs, and critical workflows.
2. Identify reliability, security, latency, scale, and cost requirements.
3. Define domain boundaries.
4. Choose the simplest viable architecture.
5. Identify failure modes and observability needs.
6. Document major decisions and trade-offs.
7. Add complexity only when justified.

## Architectural Principles

- Separation of concerns
- Explicit interfaces and contracts
- Loose coupling where it creates real value
- High cohesion
- Idempotency for retryable operations
- Observability as part of design
- Least privilege
- Backward-compatible evolution where practical
- Prefer boring technology for stable workloads

## Patterns

### Modular Monolith
Use when the domain is evolving, the team is small, or operational simplicity matters.

### Microservices
Use when independent deployment, scaling, ownership, or fault isolation justifies distributed complexity.

### Event-Driven
Use for asynchronous processing, decoupling, integrations, or durable event history.

### Queue-Based Worker
Use for long-running, bursty, retryable, or asynchronous jobs.

### API + Service Layer
Use when external interfaces need separation from business logic.

### RAG / Knowledge Retrieval
Use when AI needs grounded access to changing or private knowledge. Do not add vector search without a real retrieval problem.

## Decision Rule

**Requirement -> constraints -> simplest architecture -> measurable validation.**

## For AI Systems

This knowledge should be used for:
- Designing systems that fit actual requirements
- Selecting patterns based on constraints
- Explaining distributed-system trade-offs before adding complexity

Query examples:
- "Design a system using my preferred patterns"
- "Should this be a monolith or microservices?"
- "What failure modes should this architecture handle?"

Related topics:
- [[CODING-STANDARDS]]
- [[SECURITY]]
- [[TESTING]]
