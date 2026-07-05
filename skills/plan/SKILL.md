---
name: plan
description: Analyze a development request, produce an execution plan, and recommend whether the work should be tracked before implementation begins.
version: 0.2.0
tags:
  - workflow
  - planning
  - execution
---

# Purpose

Use this workflow before starting any implementation.

The objective is to transform a user request into a clear execution plan that can be reviewed, approved, and tracked.

The execution plan becomes the contract for implementation.

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

❌ Technical Slice

- Create components
- Update API
- Modify database

✅ Functional Slice

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

> How do we know this work is complete?

Avoid vague statements.

---

## 7. Prepare the Execution Plan

Prepare a structured execution plan containing:

- Summary
- Goal
- Scope
- Out of Scope
- Slices
- Risks
- Acceptance Criteria
- References (optional)

Present the execution plan to the user for review.

Do not implement anything.

---

## 8. Recommend Tracking

Determine whether this work should be tracked using the project's issue tracker.

Consider:

- Is this a new feature?
- Is this a bug fix?
- Does it require multiple commits?
- Does it affect the product roadmap?
- Will it likely require code review?
- Will it be useful to reference later?

Recommend one of the following:

### Create an Issue

Use when the work should be tracked as part of the project's development history.

### Continue Without an Issue

Use for small or temporary work such as:

- typo fixes
- formatting
- trivial documentation
- small refactoring
- local experiments
- short-lived spikes

Always explain your recommendation.

Do not create the issue yet.

---

## 9. Wait for Approval

Wait for explicit user approval.

Examples include:

- gas
- approve
- proceed
- continue
- looks good

Before approval:

- do not implement code
- do not modify repository files
- do not create commits
- do not create branches
- do not create pull requests
- do not create issues

---

# Execution Plan Template

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

## Tracking Recommendation

- Create an Issue
- Continue Without an Issue

Reason:

...

---

# Safety Rules

Never:

- start implementation
- modify repository files
- create commits
- create branches
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
- work has been divided into functional slices
- risks have been identified
- acceptance criteria have been defined
- an execution plan has been prepared
- a tracking recommendation has been provided
- the workflow is waiting for user approval