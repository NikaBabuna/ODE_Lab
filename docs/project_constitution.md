# Project Constitution — ODE Lab

## Role

This document defines the laws of the project.

It governs scope, architecture, quality standards, and decision authority.
All development must comply with this document.

Long-term direction is defined in Vision.
Growth model is defined in Evolution Strategy.
Core foundation is defined in Core Specification.

---

## Purpose

ODE Lab exists to develop:

1. Strong software engineering discipline
2. Deep understanding of numerical ODE methods
3. A professional-quality system suitable for presentation

All decisions must support these goals.

---

## Scope

### In Scope
- Ordinary Differential Equations (ODE)
- Initial Value Problems (IVP)
- Boundary Value Problems (BVP)
- Numerical solver implementation
- Solver diagnostics and comparison
- Interactive visualization
- Extensible architecture

### Out of Scope
- PDE solvers
- Machine learning integration
- GPU acceleration
- Large scientific computing frameworks
- Unbounded feature expansion

The system must remain focused and intentional.

---

## Architectural Principles

### Core / Interface Separation
Numerical core must remain independent from UI and visualization layers.

### Extensibility
New solvers and simulations must be addable without structural rewrites.

### Determinism
Solver behavior must be reproducible and transparent.

### Clarity
Readable, explainable implementations are preferred over cleverness.

---

## Quality Bar

The project follows professional-grade standards:

- Clean, structured code
- Strong testing discipline
- Clear documentation
- Stable main branch
- Demonstrable numerical correctness

Untested or unclear core logic is unacceptable.

---

## Learning Integrity

External references and AI tools may be used.

However:
- Implementations must be understood
- Blind copying is forbidden
- Core logic must be explainable independently

---

## Decision Authority

When uncertain:

1. Preserve clarity
2. Protect architecture
3. Avoid unnecessary expansion
4. Favor understanding over speed

This document defines project law.
