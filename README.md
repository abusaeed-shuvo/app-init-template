# App Init Template

A reusable set of engineering instructions for AI coding agents. This repository
contains no application code — it is a documentation-only template that defines
how an agent should approach building and modifying a software project.

Copy it into a new project, fill in the project-specific blanks, and point your
agent at `init.md` as the entry point.

## Repository Structure

```text
.
├── init.md              Entry point: required reading, core rules, instruction priority
└── init.md.d/           Authoritative project specification
    ├── project.md              Application brief, requirements, acceptance criteria
    ├── stack.md                Runtime, framework, allowed libraries, dependency rules
    ├── architecture.md         Structure, responsibilities, change boundaries
    ├── coding-conventions.md   Style and implementation conventions
    ├── data-contracts.md       Data formats and interfaces
    ├── testing.md              Testing strategy and expectations
    ├── error-handling.md       Error handling rules
    ├── debugging-recovery.md   Debugging and recovery procedures
    ├── security-performance.md Security and performance constraints
    └── workflow-done.md        Standard workflow, Definition of Done, git safety
```

Treat the files in `init.md.d/` as the authoritative project specification.
`init.md` is only the routing document that tells the agent what to read and how
to behave.

## Quick Start

1. Copy this repository into your new project.
2. Replace the `[TODO]` placeholders in `./init.md.d/project.md` with the actual
   project brief (name, purpose, users, requirements, non-goals).
3. Replace the `[TODO]` placeholders in `./init.md.d/stack.md` with the chosen
   runtime, language, framework, and allowed libraries.
4. Fill in `./init.md.d/architecture.md` with the intended project structure.
5. Point your AI coding agent at `./init.md` and ask it to read the required
   files before making any implementation changes.

Until steps 2–4 are done, the template is only a skeleton — the project brief is
intentionally kept separate so the template stays reusable.

## Core Operating Rules

- Do not invent requirements that conflict with the project specification.
- Do not add libraries, frameworks, services, or tooling without justification.
- Inspect existing code before changing it.
- Prefer the smallest correct change.
- Preserve working functionality.
- Never hide, suppress, or weaken an error merely to make a test pass.
- Test changes before considering them complete.
- If a decision would materially change architecture, dependencies, data
  formats, or public behavior, stop and ask the user before proceeding.

## Workflow

Work incrementally:

```text
Understand → Plan → Implement → Test → Review → Report
```

Code generation alone is not completion. Completion means the Definition of Done
in `init.md.d/workflow-done.md` has been satisfied: requirements implemented,
error cases handled, tests added and passing, no debug code left behind, and no
unrelated changes introduced.

## Instruction Priority

When instructions conflict, use this order:

1. Explicit user instruction
2. Project-specific requirements
3. Security and data-integrity requirements
4. Architecture constraints
5. Testing requirements
6. Maintainability and performance
7. Convenience

Never silently override a higher-priority rule for convenience.

## File Reference

| File | Responsibility |
| --- | --- |
| `init.md` | Entry point, required reading list, core operating rules |
| `init.md.d/project.md` | Project brief, functional/UX/technical requirements, acceptance criteria |
| `init.md.d/stack.md` | Runtime and framework boundary, allowed libraries, dependency change rule |
| `init.md.d/architecture.md` | Project structure, responsibility placement, architectural change boundary |
| `init.md.d/coding-conventions.md` | Code style and implementation conventions |
| `init.md.d/data-contracts.md` | Data formats, schemas, and interface contracts |
| `init.md.d/testing.md` | Testing strategy, coverage expectations, how to run tests |
| `init.md.d/error-handling.md` | How errors are surfaced, logged, and propagated |
| `init.md.d/debugging-recovery.md` | Debugging process and recovery from failures |
| `init.md.d/security-performance.md` | Security constraints and performance budgets |
| `init.md.d/workflow-done.md` | Standard workflow, Definition of Done, git safety rules |

## License

This project is licensed under the MIT License — see [LICENSE](LICENSE).

Copyright (c) 2026 abusaeed-shuvo
