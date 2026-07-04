---
name: post-merge
description: Synchronize the local repository after a pull request has been merged and prepare the project for the next development task.
version: 0.1.0
tags:
  - workflow
  - git
  - repository
  - maintenance
---

# Purpose

Use this workflow after a pull request has been merged.

The objective is to leave the repository in a synchronized, healthy, and predictable state so development can continue immediately.

This workflow assumes that a human has already completed the merge through the project's repository hosting platform.

# When to Use

Use this workflow after a pull request has been merged into the repository's default branch.

Typical user requests include:

- post-merge
- next
- PR merged
- already merged
- done merging

Do not use this workflow before the merge has been completed.

# Workflow

## 1. Verify Merge Status

Verify that the current work has already been merged into the repository's default branch.

If the merge cannot be confirmed:

* stop immediately
* explain why the workflow cannot continue
* do not modify the repository


## 2. Synchronize Repository

Detect the repository's default branch

Synchronize the local repository with the latest remote state.

Never overwrite local work.


## 3. Clean Up

Perform safe cleanup operations when appropriate.

Examples include:

* removing merged local branches
* pruning deleted remote branches
* cleaning temporary worktrees

Never remove branches that still contain unmerged work.


## 4. Synchronize Development Environment

Determine whether dependencies or generated files need to be synchronized.

Only perform synchronization when required.

Do not assume a specific package manager or build tool.


## 5. Verify Repository Health

Run lightweight verification suitable for the project.

Prefer:

* type checking
* linting
* quick validation

Avoid long-running verification unless recommended by the project.


## 6. Generate Session Handoff

If the project provides a dedicated handoff workflow, invoke it.
Otherwise generate a concise summary including:
* completed work
* current repository state
* recommended next step


## 7. Complete

Provide a concise completion summary including:
* repository synchronized
* cleanup completed
* environment synchronized
* verification completed
* handoff completed

Finish with:

> Ready for the next task.


# Safety Rules

Never:
* force push
* force delete branches
* overwrite local changes
* discard uncommitted work
* merge branches
* deploy applications
* modify unrelated files

Always choose the safest operation available.

If uncertain, stop and explain the situation instead of guessing.

# Tool Agnostic

Do not assume:
* the default branch is 'main'
* GitHub is used
* branch names
* package managers
* programming languages
* frameworks
* repository hosting providers

Detect the project's conventions before taking action.

# Expected Outcome

At the end of this workflow:

- the repository is synchronized
- local cleanup has been completed safely
- the development environment matches the repository
- verification has succeeded or failures have been reported
- a handoff or session summary exists
- the repository is ready for the next task