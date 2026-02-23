# ODE Lab — Workflow Bible

### Personal Engineering Doctrine & Operating System

## 1. Purpose

This document defines the working philosophy, discipline, and development process for the **ODE Lab project**.

The goal is not only to build a numerical software product, but to train the mind and habits of a high-level engineer.

This workflow exists to maximize:

* Deep understanding
* Engineering discipline
* Consistency of progress
* Code quality and clarity
* Professional presentation
* Personal mastery of numerical programming and software engineering

This is a **craftsmanship project**.
Speed matters less than clarity, correctness, and structured growth.

---

## 2. Core Principles

### 2.1 Build to Understand

All code must be written with the intent of full understanding.
No blind copying. No “magic” implementations.

If something is not understood:

* Pause
* Study
* Re-derive
* Then implement

Understanding > completion speed.

---

### 2.2 Clean Engineering Above All

Every component must be:

* Readable
* Testable
* Documented
* Structured

The repository should look like it was written by a disciplined engineering team, not a student rushing a deadline.

Clean code is not optional. It is the default state.

---

### 2.3 Incremental Construction

Nothing large is built at once.

All development happens through:

* Small isolated tasks
* Clear objectives
* Tested results
* Continuous integration into the main system

Progress must always be visible and stable.

---

### 2.4 Test Before Trust

Numerical software cannot rely on visual correctness alone.

Every solver and feature must be verified through:

* Analytic solutions where possible
* Convergence tests
* Stability checks
* Regression tests

If it is not tested, it is not complete.

---

### 2.5 Visible Professionalism

This project is also a portfolio artifact.

Every commit, file, and document should reflect:

* Order
* Structure
* Care
* Intentional design

The repository should be understandable and impressive to external reviewers.

---

## 3. Development Methodology

This project follows a **Structured Iterative Engineering** model.

It combines:

* Waterfall clarity (planned architecture)
* Agile iteration (small steps)
* Test-driven discipline (verification)
* Continuous refactoring (cleanliness)

Development proceeds in repeated cycles.

### Cycle Structure

Each development cycle consists of:

1. Design
2. Implementation
3. Verification
4. Refinement
5. Documentation

Then repeat.

No uncontrolled coding is allowed.

---

## 4. Project Structure Strategy

The system will be built as two primary layers:

### Core Engine (odelab-core)

Responsible for:

* ODE solvers
* Numerical methods
* Event detection
* Step control
* Mathematical correctness

This layer must be:

* Deterministic
* Fully tested
* UI-independent
* Cleanly documented

### Application Layer (odelab-app)

Responsible for:

* Simulation selection
* Visualization
* Parameter interaction
* User interface

This layer must:

* Use core as a dependency only
* Contain minimal numerical logic
* Focus on clarity and usability

Strict separation must be maintained.

---

## 5. Task Execution Rules

### 5.1 Task Size

All work must be broken into small, definable tasks.

A task should:

* Be completable in 30–120 minutes
* Have a clear success condition
* Produce a testable result

Large tasks must be divided.

---

### 5.2 Before Starting a Task

Before implementation:

* Understand the goal
* Identify inputs and outputs
* Define how success will be tested
* Consider edge cases

No blind coding.

---

### 5.3 During Implementation

Work with full focus.

Rules:

* No multitasking
* No rushing
* Code for clarity first
* Prefer simple correct implementations over clever ones

If confusion appears: stop and resolve it.

---

### 5.4 After Implementation

Immediately:

* Test behavior
* Refactor for clarity
* Add docstrings/comments
* Ensure style consistency
* Commit cleanly

Never leave messy code for later cleanup.

---

## 6. Testing Doctrine

Testing is integral, not optional.

### Required Test Types

**Analytical correctness tests**

* Compare with known solutions
* Verify expected accuracy

**Convergence tests**

* Error vs step size
* Confirm expected order

**Behavior tests**

* Event detection correctness
* Stability behavior
* Solver diagnostics

**Regression tests**

* Prevent future breakage

All core numerical features must include tests before being considered complete.

---

## 7. Documentation Discipline

Documentation is written continuously.

Required documentation:

* Clear README
* Design notes (`docs/design.md`)
* Numerical notes
* Usage examples
* Clean docstrings

If a future reader cannot understand the system easily, documentation is insufficient.

---

## 8. Version Control Discipline

Version control reflects engineering maturity.

Rules:

* Small, meaningful commits
* Clear commit messages
* Feature branches for new work
* Main branch always stable
* No broken main branch

Commit message style:

* `feat: implement rk4 solver`
* `test: add convergence test for rk4`
* `refactor: simplify step size controller`

---

## 9. Weekly Operating Rhythm

### Weekly Planning (start of week)

* Review roadmap
* Select current milestone
* Break into tasks
* Define goals for week

### Daily Work Session

For each session:

1. Choose one task
2. Design briefly
3. Implement
4. Test
5. Refactor
6. Commit

### Weekly Review (end of week)

* Clean documentation
* Ensure repository order
* Review progress
* Plan next steps

Consistency is more important than intensity.

---

## 10. Engineering Mindset

This project is not a race.
It is training.

Focus on:

* Precision
* Clarity
* Understanding
* Stability
* Professionalism

Work calmly and deliberately.

Every line written should move toward mastery.

---

## 11. Final Standard

When complete, this project should demonstrate:

* Strong numerical programming ability
* Professional software engineering discipline
* Clean architecture
* Thorough testing
* Clear documentation
* Thoughtful design

The finished system should reflect not only skill, but engineering character.

This document defines the standard.
All work follows it.
