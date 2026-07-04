# post-merge

Synchronize a repository after a pull request has been merged.

## Purpose

This workflow prepares the repository for the next development task by:

* synchronizing the local repository
* cleaning merged branches
* synchronizing the development environment when required
* performing lightweight verification
* generating a concise handoff summary

## Usage

Invoke the workflow after a pull request has been merged.

Typical examples include:

```text
post-merge
```

or

```text
next
```

## Workflow

1. Verify that the pull request has already been merged.
2. Synchronize the repository with the default branch.
3. Clean up merged branches when safe.
4. Synchronize the development environment if required.
5. Run lightweight verification.
6. Generate a handoff summary.
7. Report completion.

## Optional Integration

If the project provides a dedicated handoff workflow, it should be used.

Otherwise, generate a concise summary describing:

* completed work
* current repository state
* recommended next step

## License

MIT

### Maintainer

Sandi Andrian  <andrian.sandi@gmail.com>