# Workflow Bible — Personal Engineering Doctrine

## Role

This document defines how development work is performed on ODE Lab.

It governs discipline, task execution, and engineering behavior.
It does not define project scope, architecture, or long-term direction.

Those are defined in:
- Project Constitution
- Vision
- Evolution Strategy
- Core Specification

---

## Guiding Principle

Work deliberately. Build cleanly. Understand completely.

---

## Core Rules

### 1. Build for Understanding
All code must be fully understood.
Blind copying or opaque implementation is forbidden.

External references may be used, but implementations must be owned.

### 2. Incremental Construction
All development is performed in small, isolated tasks.
Large changes must be divided into verifiable steps.

### 3. Clean State Policy
The repository must remain clean at all times.
No intentional accumulation of temporary or messy structures.

### 4. Test Before Trust
Numerical behavior must be validated.
Visual correctness alone is insufficient.

---

## Task Execution Cycle

Each task must follow:

1. Clarify objective
2. Design approach briefly
3. Implement clearly
4. Verify with tests or experiments
5. Refactor for clarity
6. Commit in clean state

---

## Task Size Standard

Tasks should be completable within one focused session.
Large features must be decomposed.

---

## Commit Discipline

Commits must:
- Represent meaningful progress
- Leave the repository stable
- Avoid mixing unrelated changes
- Use clear descriptive messages

Main branch must remain stable.

---

## Session Closure Rule

Each session must end with:
- Clean code
- Passing tests
- Clear next task defined

Consistency is prioritized over intensity.
