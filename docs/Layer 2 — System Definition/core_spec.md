# Core Specification — ODE Lab

## Role

This document defines the minimal foundation system.

It describes what must exist before expansion begins.

Completion of this specification marks the end of Phase I (Foundation).

---

## Purpose of the Core

The core is the stable nucleus of ODE Lab.

It must provide:

- A working interactive laboratory
- A unified solver architecture
- A formal problem definition interface
- A stable execution pipeline
- A foundation that supports expansion without structural rewrite

After completion, development must occur around the core, not through redesign.

---

## Core Components

### 1. Solver System

Minimum solver set:

- RK4 (fixed-step baseline)
- RK45 (adaptive solver)
- Backward Euler (implicit/stiff baseline)

Each solver must:
- Conform to a unified interface
- Operate on generic problem definition
- Return standardized solution objects
- Provide diagnostic data

---

### 2. Problem Definition Interface

Each problem must define:

- State dimension
- Derivative function f(t, y, params)
- Parameter set
- Initial conditions
- Optional event functions

Problems must remain solver-independent.

---

### 3. Execution Engine

Unified execution interface:

solve(problem, solver, config) → solution

Solution must contain:
- Time values
- State values
- Diagnostics
- Event results (if applicable)

Core engine must not depend on UI.

---

### 4. Event System

Minimum support:
- Zero-crossing detection
- Stop-on-event capability
- Accurate event time approximation

---

### 5. Minimal Interactive Lab

Must allow:

- Selection of simulation
- Selection of solver
- Parameter adjustment
- Execution
- Visualization of results

Required visualizations:
- Time-series plots
- Phase plots
- Basic solver diagnostics

UI must remain thin and separate from core.

---

### 6. Initial Simulation Set

Core includes:

- Projectile with event detection
- Pendulum
- Lorenz attractor
- Van der Pol oscillator

---

## Explicitly Excluded from Core

- BVP solvers
- Symplectic methods
- DSL / scripting system
- Advanced visualization tools
- Performance optimization
- Plugin auto-discovery

These belong to Phase III.

---

## Definition of Core Completion

Core is complete when:

- Multiple solver types operate under unified interface
- Simulations run correctly across solvers
- Events function correctly
- Visualization works
- New solver can be added without modifying existing ones
- New simulation can be added without modifying solver code
- System is stable and understandable
