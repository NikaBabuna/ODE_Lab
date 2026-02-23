# Structured Solo Project Method

### A Layered Workflow for Building Complex Technical Systems

## Purpose

This document defines the structured workflow method used to design and build ODE Lab.
It describes how a complex solo-engineered system is defined, constructed, stabilized, and expanded without chaos or drift.

This method separates:

* levels of abstraction
* phases of development
* types of decisions

The goal is to create clarity, stability, and controlled progress from idea to long-term evolution.

This document explains:

* what must be defined
* where it is defined
* how all documents relate
* how work flows from abstract definition to implementation

---

# Core Principle

Do not mix levels of abstraction or phases of development.

Each layer defines something different.
Each phase requires a different mode of operation.

Clarity emerges when:

* high-level decisions remain stable
* implementation happens within defined boundaries
* expansion occurs only after a stable core exists

---

# Part I — Layered Project Architecture

The method organizes a project into five layers, from highest abstraction to lowest execution.

Each layer answers different questions and contains different documents.

Higher layers constrain lower layers.
Lower layers must never contradict higher ones.

---

## Layer 1 — Doctrine (Operating Environment)

### Role

Defines the identity and governing environment of the project.

This layer establishes the stable conceptual foundation in which all work occurs.

### Defines

* Purpose of the project
* Scope boundaries
* Quality standards
* Architectural principles
* Personal engineering discipline
* Long-term direction
* Evolution model

### Documents

* Workflow Bible
* Project Constitution
* Vision
* Evolution Strategy

### Characteristics

* Highest abstraction
* Rarely modified
* Independent of features and implementation
* Governs all lower layers

### Questions answered

* Why does this project exist?
* What is it allowed to become?
* How should work be performed?
* How will it evolve over time?

---

## Layer 2 — System Definition

### Role

Defines the concrete system that must be built within the doctrine.

This layer translates abstract direction into a minimal structural target.

### Defines

* The minimal core system
* Required capabilities of the foundation
* What must exist before expansion begins
* What is excluded from the core
* Criteria for core completion

### Documents

* Core Specification

### Characteristics

* Stable once defined
* Rarely modified
* Must comply with Doctrine

### Questions answered

* What are we actually building first?
* What constitutes a stable foundation?
* When is the core complete?

---

## Layer 3 — Operational Strategy

### Role

Defines how development operates within each evolution phase.

This layer translates high-level evolution into rules of engagement.

### Defines

* How work is conducted in each phase
* How features are implemented during expansion
* How transitions between phases occur
* What is allowed or forbidden per phase

### Documents

* Operational Strategy
* Feature Implementation Protocol

### Phase Behavior

**Phase I — Foundation**
Strict roadmap-driven construction.

**Phase II — Stabilization**
Formal refinement and structural cleanup.

**Phase III — Controlled Expansion**
Backlog-driven, single-feature iterative growth.

### Characteristics

* Procedural and stable
* Applies throughout project life
* Must comply with Layers 1 and 2

### Questions answered

* How do we behave during each phase?
* How are features selected and added?
* How do we move between phases?

---

## Layer 4 — Execution

### Role

Defines structured plans and progress within a phase.

This layer translates strategy into concrete action.

### Documents

During Phase I:

* Core Roadmap
* Core Progress Tracker

During Phase III:

* Feature Backlog

### Defines

* Work sequence
* Milestones
* Current progress
* Feature queue

### Characteristics

* Changes as development progresses
* Archived or replaced when phases change
* Must comply with all higher layers

### Questions answered

* What is the current plan?
* What comes next?
* What remains to be done?

---

## Layer 5 — Daily Implementation

### Role

Represents active engineering work.

This is where code is written and features are implemented.

### Artifacts

* Task lists
* Temporary notes
* Experiments
* Implementation code

### Characteristics

* Continuously changing
* Flexible and adaptive
* Lowest abstraction
* Constrained by all higher layers

### Questions answered

* What am I building today?
* What is the next small step?

---

# Part II — Phase-Based Development Workflow

The project evolves through three distinct phases.
Each phase requires a different operating mode.

---

## Phase I — Foundation

### Objective

Build the minimal stable core defined in the Core Specification.

### Mode

Strict roadmap-driven construction.

### Rules

* Work only on roadmap-defined tasks
* No expansion features
* No unrelated improvements
* Focus on core completion criteria

### Completion

Occurs only when all core completion criteria are satisfied.

---

## Phase II — Stabilization

### Objective

Refine and harden the core system.

### Mode

Formal cleanup and strengthening.

### Allowed

* Refactoring
* Test improvement
* Documentation
* Structural clarification

### Forbidden

* New major features
* Expansion systems

### Completion

When the core is stable, clean, and extensible.

---

## Phase III — Controlled Expansion

### Objective

Expand system toward vision without destabilizing the core.

### Mode

Backlog-driven iterative development.

### Rules

* One feature at a time
* No parallel feature development
* Preserve core stability
* Avoid architectural rewrites
* Each feature must reach clean completion

### Structure

Select feature → implement → stabilize → repeat

This phase is unbounded and continuous.

---

# Part III — Workflow Hierarchy

All work must follow this downward flow:

Doctrine
→ defines environment and limits

System Definition
→ defines core structure

Operational Strategy
→ defines behavior per phase

Execution
→ defines current plan

Daily Implementation
→ produces working code

Decisions must move downward through this hierarchy.

---

# Stability Model

Layer 1 — Almost never changes
Layer 2 — Rarely changes
Layer 3 — Stable procedural rules
Layer 4 — Changes per phase
Layer 5 — Changes constantly

This separation preserves clarity and prevents drift.

---

# Final Principle

Clarity at higher layers enables freedom at lower layers.

By defining doctrine, system boundaries, and operational rules first,
implementation becomes focused and controlled rather than chaotic.

This method allows a complex solo-engineered project to move from idea to stable core and into long-term expansion without loss of direction or structural integrity.
