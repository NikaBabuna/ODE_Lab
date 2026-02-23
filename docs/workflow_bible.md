# Workflow Bible — Personal Engineering Doctrine

## Purpose

This document defines how development work is performed on ODE Lab.
It governs discipline, task execution, and daily engineering behavior.

It does not define project scope or architecture.
It defines how work is done.

---

## Core Principles

### Build for Understanding

All code must be written with full comprehension.
No blind copying or opaque implementation is allowed.

Understanding takes priority over speed.

### Incremental Construction

All work is performed in small, isolated tasks.
Large changes are divided into clear steps with verifiable outcomes.

### Clean State Policy

Code must remain clean and readable at all times.
No intentional accumulation of messy or temporary structures.

### Test Before Trust

All numerical behavior must be verified through tests or experiments.
Visual correctness alone is insufficient.

---

## Task Execution Cycle

Each task follows this sequence:

1. Understand goal and constraints
2. Design approach briefly
3. Implement clearly
4. Test and verify behavior
5. Refactor for clarity
6. Commit in clean state

No uncontrolled coding is allowed.

---

## Task Size Standard

Tasks must be small and well-defined.
A task should typically be completable in one focused session.

Large features must be divided into smaller steps.

---

## Commit Discipline

Commits must:

* Represent meaningful progress
* Leave repository in clean state
* Use clear descriptive messages
* Avoid mixing unrelated changes

Main branch must remain stable.

---

## Testing Discipline

Core numerical code requires:

* Analytical or reference validation
* Behavioral verification
* Regression protection where appropriate

Untested core logic is considered incomplete.

---

## Session Rhythm

Each work session:

* Select one defined task
* Complete full execution cycle
* Leave system clean and stable

Consistency is prioritized over intensity.

---

## Guiding Rule

Work calmly, deliberately, and cleanly.

Each session should move the system forward
while strengthening engineering discipline.
