# Feature Implementation Protocol — Phase III

## Purpose

This document defines the exact process for implementing new features during Phase III (Controlled Expansion).

It ensures that expansion remains modular, disciplined, and architecturally safe.

This protocol applies only during Phase III.

---

# Core Principle

Only one feature may be actively developed at a time.

Expansion is sequential and isolated.

---

# Step 1 — Feature Selection

A feature must originate from the maintained feature backlog.

Before development begins, the feature must be:

- Clearly named
- Clearly scoped
- Described in one paragraph
- Verified as aligned with Vision
- Confirmed as compliant with Constitution

If scope is unclear, it must be refined before implementation begins.

---

# Step 2 — Isolation Check

Before writing code, verify:

1. Can this feature be implemented without modifying core architecture?
2. Does it require rewriting existing systems?
3. Does it introduce cross-cutting dependencies?

If the feature requires structural modification of the core,
it must be reconsidered or split into smaller units.

Core stability has priority over feature ambition.

---

# Step 3 — Feature Design Note

Create a short design note (temporary document or section in backlog):

- What is being added?
- Which modules are affected?
- What interfaces are used?
- What new interfaces (if any) are introduced?

No large design documents required.
Clarity is the goal.

---

# Step 4 — Implementation

Rules during implementation:

- Work only on this feature.
- Do not mix unrelated improvements.
- Preserve existing behavior.
- Maintain test coverage.
- Avoid opportunistic refactoring unless necessary.

If refactoring becomes necessary,
it must remain localized and justified.

---

# Step 5 — Integration Verification

Before declaring feature complete:

- System builds and runs cleanly.
- All existing functionality remains intact.
- No regressions introduced.
- Feature works as intended.
- Code remains readable and modular.

If instability appears, stabilization takes precedence.

---

# Step 6 — Completion Declaration

A feature is complete only when:

- Implementation is clean.
- Tests (if applicable) are written.
- Documentation updated (if needed).
- No known structural concerns remain.

Only then may the next feature be selected.

---

# Forbidden During Phase III

- Parallel feature development
- Major architectural rewrites
- Introducing instability into the core
- Leaving partially implemented features in main branch

---

# Expansion Cycle

Phase III follows a strict cycle:

Select Feature  
→ Design Brief  
→ Implement  
→ Verify  
→ Stabilize  
→ Repeat

No overlapping cycles.

---

# Stability Rule

At all times during Phase III, the system must remain:

- Runnable
- Stable
- Understandable

Expansion must never degrade the nucleus built in Phase I.
