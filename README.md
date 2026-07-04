# Boring Code

> Make AI coding boring.

Opinionated workflow skills for AI coding agents.

boring-code provides reusable workflows that eliminate repetitive prompts and standardize AI-assisted software development.

## Why?

AI coding agents are excellent at writing code, but developers still repeat the same operational instructions:

* Create a plan.
* Start implementing.
* Create a pull request.
* Update the default branch.
* Generate a handoff.

These are workflows, not one-off prompts.

Boring Code turns them into reusable skills.

## Philosophy

Software development should be boring.

Not because it lacks creativity, but because good engineering is:

* Predictable
* Repeatable
* Reviewable
* Safe
* Easy to hand over

AI should automate operational repetition while leaving engineering decisions to humans.

## Principles

### Human in Control
* Humans review.
* Humans approve.
* Humans merge.
* AI assists.

### Workflow over Prompts
A workflow defines:
* intent
* sequence
* safety
* expected outcome

### Tool Agnostic

Workflows should adapt to the current project instead of assuming:

* Git provider
* branch names
* package managers
* programming languages
* frameworks

## Available Workflows

| Workflow     | Description                                                                                          | Status |
| ------------ | ---------------------------------------------------------------------------------------------------- | ------ |
| `post-merge` | Synchronize the local repository after a pull request has been merged and prepare for the next task. | Stable |

## Example

Instead of writing:

```text
The pull request has been merged.

Update the repository.

Clean local branches.

Synchronize dependencies.

Run verification.

Generate a handoff.
```

Simply use:

```text
post-merge
```

## Roadmap

Upcoming workflows include:

* plan
* gas
* ship
* next
* review
* release

## Contributing

Contributions are welcome.

Please open an issue before proposing a new workflow so the design can be discussed first.

## License

MIT

### Maintainer
Sandi Andrian <andrian.sandi@gmail.com>