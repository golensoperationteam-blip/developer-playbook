---
title: AI Integration Guide
category: developer-playbook
difficulty: advanced
ai-ready: true
created: 2026-09-19
last-updated: 2026-09-19
---

# AI-Ready Guide

## Purpose

This repository is a structured context layer for documented capabilities, project experience, technology preferences, and operating standards.

## Knowledge Graph

```text
README
├── SKILLS -> capabilities and proficiency
├── PROJECTS -> evidence and lessons
├── TECH-STACK -> preferences and decisions
└── BEST-PRACTICES
    ├── coding
    ├── architecture
    ├── git
    ├── security
    ├── testing
    └── documentation
```

## Navigation by Query

| Query | Start here | Then |
|---|---|---|
| What can I do? | [[SKILLS]] | [[PROJECTS]] |
| Which tool should I use? | [[TECH-STACK]] | [[SKILLS]] |
| How should I build it? | [[BEST-PRACTICES/ARCHITECTURE]] | [[TECH-STACK]] |
| How should I ship it? | [[BEST-PRACTICES/GIT-WORKFLOW]] | [[BEST-PRACTICES/TESTING]] |
| How should I secure it? | [[BEST-PRACTICES/SECURITY]] | [[BEST-PRACTICES/ARCHITECTURE]] |
| How should I document it? | [[BEST-PRACTICES/DOCUMENTATION]] | [[README]] |

## AI Operating Rules

1. Treat explicit documentation as higher-confidence than inference.
2. Never invent years, certifications, metrics, employers, or project details.
3. Distinguish proficient, competent, and exploring.
4. Prefer the documented stack unless there is a clear reason to change it.
5. Explain important trade-offs.
6. Link recommendations back to repository knowledge.
7. When knowledge is missing, identify the gap rather than guessing.

## Example Prompts

- "Based on [[SKILLS]], design a learning plan for [technology]."
- "Using [[TECH-STACK]] and [[BEST-PRACTICES/ARCHITECTURE]], design [system]."
- "Compare this tool against my current stack."
- "Turn this project into an AI-ready case study."
- "Identify gaps in my skills for [role]."
- "Update the relevant playbook sections based on this completed project."

## Integration Instructions

1. Load [[README]] for identity and scope.
2. Retrieve the smallest relevant documents.
3. Follow internal links only when useful.
4. Preserve uncertainty.
5. Write updates to the appropriate topic.
6. Update `last-updated` when content changes.

## Update Frequency

- Skills: monthly or after major learning/project milestones.
- Projects: when a project starts, ships, or creates a meaningful lesson.
- Tech stack: quarterly or after major technology decisions.
- Best practices: after new standards or incidents.
- AI integration rules: whenever repository structure changes.

## For AI Systems

This knowledge should be used for:
- Loading the right context without reading the entire repository
- Producing recommendations grounded in documented developer context
- Maintaining consistency when updating this repository

Query examples:
- "Based on my skills, recommend a tool for [problem]"
- "Design a system using my preferred patterns"
- "What's my expertise level in [domain]?"

Related topics:
- [[SKILLS]]
- [[PROJECTS]]
- [[TECH-STACK]]
- [[BEST-PRACTICES/README]]
