# ODE Lab — Core Roadmap

### Phase I: Foundation Campaign

## Purpose

This roadmap defines the structured development path for building the ODE Lab core.

The objective of this phase is to construct a stable, extensible nucleus that supports all future expansion without structural redesign.

This roadmap is finite.
It ends when the core is complete and stable.

After completion, roadmap-driven development ends and the project moves into expansion mode guided by a feature backlog rather than a fixed plan.

This roadmap operates within the constraints defined by:

* Project Constitution
* Vision
* Evolution Strategy
* Core Specification

---

# Timeline and Intensity

Estimated duration: ~4 weeks
Intensity: High (15–25 hours/week)
Mode: Progressive difficulty with controlled stabilization

The roadmap is designed as a focused engineering campaign rather than an open-ended development cycle.

---

# Week 1 — System Activation (Vertical Slice)

## Goal

Bring the laboratory to life with a minimal end-to-end working system.

The objective is to establish a functioning pipeline from solver to visualization.

## Deliverables

* Repository structure finalized
* Core execution pipeline defined
* RK4 solver implemented (baseline)
* One simple simulation implemented (pendulum or analytic test)
* Minimal problem definition interface created
* Basic Streamlit interface:

  * select simulation
  * run solver
  * display time-series plot

## Constraints

* No adaptive stepping yet
* No implicit methods
* No event detection
* No architectural perfectionism

Focus on existence, not completeness.

## Completion Condition

A working system capable of running a simulation and displaying results interactively.

At this point:
ODE Lab exists as a functioning system.

---

# Week 2 — Solver Architecture and Adaptive Methods

## Goal

Establish a serious solver architecture and implement adaptive integration.

## Deliverables

* Unified solver interface defined
* RK4 refactored into final solver structure
* RK45 adaptive solver implemented
* Error estimation and step control implemented
* Step rejection and tolerance handling implemented
* Solver diagnostics tracking added
* Convergence verification scripts created
* Comparison runs between RK4 and RK45

## Focus

Numerical correctness and architectural clarity.

All solver implementations must:

* follow unified interface
* operate on generic problem definition
* return consistent solution structure

## Completion Condition

Adaptive solver functioning correctly with verified convergence behavior.

---

# Week 3 — Implicit Methods and Event System

## Goal

Introduce stiffness handling and event-driven integration.

## Deliverables

* Backward Euler solver implemented
* Newton iteration for implicit steps implemented
* Event detection system implemented:

  * zero-crossing detection
  * stop-on-event support
  * event time approximation
* Projectile simulation with event detection added
* Van der Pol oscillator added for stiffness testing

## Focus

Structural completeness of solver engine.

System must now support:

* fixed-step
* adaptive
* implicit/stiff
* event-driven integration

## Completion Condition

Multiple solver types operate correctly across multiple systems with event handling functional.

---

# Week 4 — Stabilization and Core Completion

## Goal

Stabilize, clean, and finalize the core system.

## Deliverables

* Codebase refactored for clarity and consistency
* Module separation finalized
* Solver interchangeability verified
* Lorenz attractor simulation added
* UI clarity improved
* Solver diagnostics panel added
* Tests strengthened
* Documentation updated

## Focus

Stability, readability, and architectural cleanliness.

No major new features introduced.

## Completion Condition

Core meets all criteria defined in Core Specification:

* Unified solver architecture stable
* Multiple simulations running correctly
* Events functioning
* Visualization working
* New solver can be added without modifying existing solvers
* New simulation can be added without modifying solver code
* System understandable and clean

At this point:

Phase I (Foundation) is complete
Phase II (Stabilization) is considered complete
Project enters Phase III (Controlled Expansion)

---

# After Core Completion

This roadmap terminates upon core completion.

Future development follows a flexible expansion model guided by:

* Vision
* Evolution Strategy
* Feature backlog (non-roadmapped)

No fixed roadmap governs expansion phase.

---

# Guiding Principle

Build with intensity.
Stabilize with discipline.
Complete the core decisively.

Once complete, expansion becomes modular and unbounded.
