# Week 1 Plan — ODE Lab Foundation Campaign

## Dominant Objective

Bring ODE Lab to life by implementing:

* RK4 solver
* Pendulum simulation
* Minimal execution pipeline
* Basic Streamlit visualization

At the end of Week 1, the system must be able to:

> Run a pendulum simulation using the custom RK4 solver and display results in the app.

Alive > perfect.

---

# Scope of Week 1

This week focuses on a minimal vertical slice:

Problem → Solver → Execution → Visualization

Only one solver.
Only one simulation.
No expansion features.

---

# Technical Target

### Solver

* Fixed-step RK4
* Simple configuration (t0, t_end, step size)
* Returns time and state arrays

### Simulation

Pendulum system:

θ'' + (g/L) sin(θ) = 0

Converted to first-order system:

dθ/dt = ω
dω/dt = -(g/L) sin(θ)

Parameters:

* g = 9.81
* L = 1

Initial conditions:

* θ = 1 rad
* ω = 0

### Visualization

Minimal Streamlit interface:

* Run simulation button
* Time series plot (θ vs t)
* Phase plot (θ vs ω)

No styling required.

---

# Weekly Deliverables

## A. Project Skeleton

* [ ] Create repository structure
* [ ] Define core folder layout
* [ ] Create basic Problem abstraction
* [ ] Create minimal execution pipeline structure
* [ ] Ensure project runs without errors

---

## B. RK4 Solver

* [ ] Implement RK4 step function
* [ ] Implement integration loop
* [ ] Test on simple ODE (e.g., dy/dt = -y)
* [ ] Return standardized solution format

---

## C. Pendulum Simulation

* [ ] Implement pendulum system
* [ ] Run simulation through RK4
* [ ] Validate general behavior
* [ ] Ensure clean separation from solver

---

## D. Minimal UI

* [ ] Create Streamlit app
* [ ] Add run button
* [ ] Plot time series
* [ ] Plot phase diagram
* [ ] Confirm end-to-end functionality

---

## E. Stabilization

* [ ] Refactor obvious structural issues
* [ ] Remove temporary debug code
* [ ] Add basic comments/docstrings
* [ ] Ensure repository remains clean
* [ ] Confirm system runs reliably

---

# Constraints

Do NOT:

* Implement adaptive solvers
* Implement implicit methods
* Add event detection
* Overdesign architecture
* Optimize performance
* Add additional simulations
* Expand beyond roadmap

Stay strictly within Week 1 objective.

---

# Weekly Success Criteria

Week 1 is successful if:

* The pendulum simulation runs using the custom RK4 solver
* The app displays correct plots
* Codebase remains clean and understandable
* Core architecture direction is preserved

Nothing more is required.

---

# Mindset for Week 1

This is ignition.

The goal is not sophistication.
The goal is existence.

Build something real.
Keep it clean.
Protect the foundation.
