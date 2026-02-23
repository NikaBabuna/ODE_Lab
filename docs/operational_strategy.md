# Operational Strategy — ODE Lab

## Purpose

This document defines how development operates within each evolution phase of ODE Lab.

It translates the high-level Evolution Strategy into concrete rules of engagement.

It does not define:

* project purpose
* architecture
* roadmap details
* feature lists

Those are defined elsewhere.

This document defines how work is conducted within each phase.

---

# Phase Structure

ODE Lab evolves through three phases:

Phase I — Foundation
Phase II — Stabilization
Phase III — Controlled Expansion

Each phase has a distinct mode of operation.

Development behavior must change according to the active phase.

---

# Phase I — Foundation

## Objective

Construct the minimal stable core defined in the Core Specification.

## Operating Mode

Strict roadmap-driven execution.

All work must follow the Core Roadmap.
No spontaneous features or deviations are allowed.

## Rules

1. Work only on items defined in the roadmap.
2. Do not introduce expansion features.
3. Do not pursue optional improvements outside roadmap scope.
4. Architectural clarity takes precedence over speed.
5. All progress must move toward core completion criteria.

## Tools

* Core Roadmap (primary guide)
* Core Progress Tracker (status visibility)
* Task list (daily execution)

## Exit Condition

Phase I ends only when all core completion criteria defined in the Core Specification are satisfied.

Transition is not time-based.
It is criteria-based.

---

# Phase II — Stabilization

## Objective

Refine and harden the core system produced in Phase I.

## Operating Mode

Formal stabilization pass.

Focus on clarity, reliability, and structural cleanliness.

## Allowed Activities

* Refactoring for readability and structure
* Strengthening tests
* Documentation improvement
* Verifying extensibility
* Removing inconsistencies

## Forbidden Activities

* New major features
* Expansion systems
* Architectural experimentation

## Exit Condition

Phase II ends when:

* Core architecture feels stable
* Codebase is clean and understandable
* Extensibility works in practice
* No structural concerns remain

Transition requires deliberate confirmation.

---

# Phase III — Controlled Expansion

## Objective

Expand the system toward the long-term Vision without compromising the core.

## Operating Mode

Backlog-driven iterative development.

No fixed roadmap governs this phase.

## Feature Selection

All work must come from a maintained feature backlog.

Features are implemented one at a time as isolated additions.

Each addition must:

* Respect existing architecture
* Avoid core rewrites
* Remain modular
* Preserve system clarity

## Rules

1. Only one expansion feature should be actively developed at a time.
2. Each feature must reach clean completion before the next begins.
3. Core stability must never be compromised.
4. Large architectural shifts are discouraged.

## Structure

Phase III is unbounded and continuous.

Development proceeds through:
select feature → implement → stabilize → repeat.

No formal completion point exists for this phase.

---

# Phase Transition Rules

Transitions between phases are strict and criteria-based.

Phase I → Phase II
Occurs only when core completion criteria are fully satisfied.

Phase II → Phase III
Occurs only after deliberate stabilization pass confirms core reliability.

No phase transition is time-driven or arbitrary.

---

# Guiding Principle

At any moment, development must clearly belong to one phase.

Do not mix operating modes between phases.

Strict construction during foundation.
Strict refinement during stabilization.
Controlled freedom during expansion.
