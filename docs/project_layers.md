# Project Layers — ODE Lab

## Purpose

This document defines the abstraction layers of the ODE Lab project.

Its purpose is to clarify:
- Where decisions belong
- How documents relate to one another
- How abstraction flows into execution
- What changes frequently and what must remain stable

This structure prevents overlap, drift, and structural confusion.

---

# Layer 1 — Foundational Doctrine

## Role

Defines the identity and governing laws of the project.

This layer establishes:
- Purpose
- Scope
- Quality standards
- Architectural principles
- Growth philosophy
- Personal engineering discipline

It defines the “physics” of the project.

## Documents

- Workflow Bible
- Project Constitution
- Vision
- Evolution Strategy

## Characteristics

- Rarely modified
- High abstraction
- Governs all lower layers
- Independent of specific features

## Answers

- Why does this project exist?
- What is it allowed to be?
- What are its long-term intentions?
- How does it grow?
- How is work performed?

---

# Layer 2 — System Definition

## Role

Defines the concrete system that must be built before expansion begins.

This layer translates vision into a minimal structural design.

## Documents

- Core Specification

## Characteristics

- Stable once defined
- Defines architectural boundaries of the foundation
- Must comply with Layer 1

## Answers

- What must exist before expansion?
- What is the minimal nucleus of the system?
- What capabilities are required in the foundation?

---

# Layer 3 — Execution Strategy (Phase I Only)

## Role

Defines how the core system will be constructed.

This layer exists only during Phase I (Foundation).

## Documents

- Core Roadmap
- Core Progress Tracker

## Characteristics

- Temporary
- Ordered and milestone-driven
- Removed or archived after core completion
- Must comply with Layers 1 and 2

## Answers

- In what sequence is the core built?
- What are the milestones?
- What is the current progress?

---

# Layer 4 — Daily Execution

## Role

Defines immediate work and operational tasks.

This layer represents active implementation.

## Artifacts

- Task lists
- Scratch notes
- Temporary design notes
- Experimental code

## Characteristics

- Continuously changing
- Ephemeral
- Lowest abstraction
- Constrained by all higher layers

## Answers

- What am I building right now?
- What is the next small step?

---

# Layer Interaction Rules

1. Lower layers must never contradict higher layers.
2. Higher layers must not micromanage lower layers.
3. Changes to Layer 1 require deliberate reconsideration.
4. Layer 3 is temporary and ends after core completion.
5. Layer 4 is allowed to be flexible and adaptive.

---

# Abstraction Flow

Foundational Doctrine
    ↓
System Definition
    ↓
Execution Strategy
    ↓
Daily Execution

Decisions must move downward through this hierarchy.

---

# Stability Model

Layer 1 — Almost never changes  
Layer 2 — Changes rarely  
Layer 3 — Exists only during core construction  
Layer 4 — Changes constantly  

This separation preserves structural clarity and prevents chaos.
