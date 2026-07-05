---
name: plan
description: Analyze a development request, produce an execution plan, and prepare an issue for implementation.
version: 0.1.0
tags:
  - workflow
  - planning
  - issue
---

# Purpose

Use this workflow before starting any implementation.

The objective is to transform a user request into a clear execution plan that can be reviewed, approved, and tracked.

The final deliverable is an execution issue that becomes the source of truth for implementation.

Never begin implementation during this workflow.

---

# Workflow

## 1. Understand the Request

Understand the user's objective.

Identify:

- desired outcome
- business value
- constraints
- success definition

Only ask questions when critical information is missing.

Avoid unnecessary clarification.

---

## 2. Inspect the Project

Inspect the project before making implementation decisions.

Understand:

- project structure
- architecture
- coding conventions
- existing documentation
- similar implementations
- dependencies

Do not assume the repository structure.

---

## 3. Determine Scope

Define:

- objective
- in scope
- out of scope
- assumptions
- dependencies

Keep the scope focused.

---

## 4. Break Into Slices

Divide the work into the smallest independently completable slices.

Each slice should:

- deliver measurable progress
- be reviewable
- have a clear objective

Avoid implementation details.

Prefer functional slices over technical tasks.

Example:

❌

- create components
- update API
- modify database

Better:

✅

- Support user authentication
- Display conversation history
- Track task cost

---

## 5. Assess Risks

Identify possible risks including:

- breaking changes
- migration
- compatibility
- performance
- security
- unknown areas

Explain why each risk exists.

---

## 6. Define Acceptance Criteria

Acceptance criteria must be observable.

Each criterion should answer:

"How do we know this work is complete?"

Avoid vague statements.

---

## 7. Prepare Execution Issue

Prepare an issue using the project's preferred issue tracker.

The issue should contain:

- Summary
- Goal
- Scope
- Out of Scope
- Slices
- Risks
- Acceptance Criteria
- References (optional)

Present the issue to the user for review.

Do not create the issue yet.

---

## 8. Wait For Approval

Wait for explicit user approval.

Examples include:

- gas
- approve
- proceed
- looks good
- continue

Before approval:

- do not implement code
- do not modify files
- do not create commits
- do not create branches
- do not create pull requests
- do not create issues

---

# Execution Issue Template

## Summary

...

## Goal

...

## Scope

...

## Out of Scope

...

## Slices

- [ ]

- [ ]

- [ ]

## Risks

...

## Acceptance Criteria

- [ ]

- [ ]

## References

...

---

# Safety Rules

Never:

- start implementation
- modify repository files
- create commits
- create pull requests
- create issues without approval
- skip repository inspection

Always validate assumptions before planning.

---

# Expected Outcome

The workflow is complete when:

- the request has been understood
- repository analysis has been completed
- scope has been defined
- work has been divided into slices
- risks have been identified
- acceptance criteria have been defined
- an execution issue has been prepared
- the workflow is waiting for user approval