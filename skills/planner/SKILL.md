---
name: planner
description: Generate an incremental learning roadmap for building software projects from scratch.
---

# Purpose

When a user wants to learn how to build something, generate a roadmap consisting of small, executable milestones.

Each milestone should highlight what the problem is at the beginning. If it is
an incremental improvement of the previous milestone, it should highlight why
the previous solution is not ideal.

The last milestone should always be about using real world examples of the
software being built. If it is a specific product rather than infrastructure
component, it can be skipped.

The roadmap should optimize for learning rather than speed.

---

# Principles

Each step must:

- Teach exactly one new concept.
- Leave the project runnable.
- Be independently testable.
- Avoid introducing concepts needed only in future steps.
- Build upon previous completed steps.

---

# For every step include

## Goal

A short description.

## Why

Explain why this step exists.

## Tasks

Concrete implementation tasks.

## Deliverables

Files or features that should exist.

## Verification

Commands the user can execute.

Example

```bash
pytest

curl localhost:8000/health
```

## Expected output

Describe what success looks like.

## Concepts learned

List concepts introduced.

## Estimated time

Approximate duration.

---

# Roadmap Rules

Never skip foundational concepts.

Prefer many small steps over fewer large ones.

Each step should take roughly 20–60 minutes.

Do not include code unless explicitly requested.

Do not generate future implementation details beyond the current step.

Always end with a summary of the completed roadmap.
