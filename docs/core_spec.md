# ODE Lab — Minimal Core Specification

## Purpose of the Core

The core is the stable nucleus of ODE Lab.

It must provide:

* a working interactive laboratory
* a clean solver architecture
* a stable problem definition system
* an extensible foundation for future expansion

After the core is complete and stabilized, all future development must occur **around** it, not through structural rewrites.

The core must be sufficient to support long-term evolution toward the full vision without requiring redesign.

---

# Core Design Principles

The core must ensure:

1. New solvers can be added without modifying existing solvers
2. New simulations can be added without modifying solver code
3. Visualization can expand without altering numerical core
4. Execution pipeline remains stable and consistent
5. System remains understandable and clean

If any future feature requires rewriting core structure, the core is considered incomplete.

---

# Core Components

## 1. Solver System

The solver system must support multiple solver types through a unified interface.

Minimum solver set:

* RK4 (fixed-step baseline)
* RK45 (adaptive step solver with error control)
* Backward Euler (implicit/stiff baseline)

Each solver must:

* conform to common interface
* operate on generic problem definition
* return standardized solution object
* provide diagnostic data (steps, rejects, etc.)

No solver may depend on specific simulations.

---

## 2. Problem Definition Interface

A formal abstraction must exist for defining dynamical systems.

Each problem must define:

* state dimension
* derivative function f(t, y, params)
* parameter set
* initial conditions
* optional event functions

Problem definitions must be solver-independent.

Adding a new simulation must require only creation of a new problem module.

---

## 3. Execution Engine

A unified execution pipeline must exist:

solve(problem, solver, config) → solution

Where solution contains:

* time values
* state values
* solver diagnostics
* event results if applicable

Execution must be deterministic and solver-agnostic.

No UI or visualization logic in core engine.

---

## 4. Event System

Core must support event detection.

Minimum requirement:

* zero-crossing detection
* ability to stop integration on event
* accurate event time approximation

This validates extensibility for future advanced features.

---

## 5. Visualization Interface (Minimal Lab)

Core must include a minimal interactive interface allowing:

* selection of simulation
* selection of solver
* parameter adjustment
* execution of simulation
* visualization of results

Required visualizations:

* time-series plots
* phase plots (where applicable)
* basic solver diagnostics display

Interface must remain thin and separate from numerical core.

Purpose is usability and validation, not visual sophistication.

---

## 6. Initial Simulation Set

Core must include a small curated set of systems:

* Projectile with event detection
* Pendulum
* Lorenz attractor
* Van der Pol oscillator

These provide coverage for:

* events
* chaos
* stiffness
* periodic systems

Additional simulations belong to expansion phase.

---

# Explicitly Excluded from Core

The following are not part of core and must not delay completion:

* BVP solvers
* Symplectic integrators
* Custom scripting or DSL
* Advanced visualization tools
* Performance optimization
* Plugin auto-discovery systems
* Large simulation libraries
* Public packaging concerns

These belong to expansion phase.

---

# Definition of Core Completion

The core is complete when:

* Multiple solver types operate through unified interface
* Simulations run correctly across different solvers
* Events function correctly
* Results can be visualized interactively
* New solver can be added without modifying existing code
* New simulation can be added without modifying solver code
* System is stable, clean, and understandable

At this point:

Phase I (Foundation) ends
Phase II (Stabilization) begins

All future development becomes expansion around a stable nucleus.
