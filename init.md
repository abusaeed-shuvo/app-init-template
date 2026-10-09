# Application Initialization

## Purpose

This file is the entry point for the project's engineering instructions.

The detailed project rules are stored in `./init.md.d/`. Treat those files as the
authoritative project specification.

## Required Reading

Before making implementation changes, read:

1. `./init.md.d/project.md`
2. `./init.md.d/stack.md`
3. `./init.md.d/architecture.md`
4. `./init.md.d/coding-conventions.md`
5. `./init.md.d/data-contracts.md`
6. `./init.md.d/testing.md`
7. `./init.md.d/error-handling.md`
8. `./init.md.d/debugging-recovery.md`
9. `./init.md.d/security-performance.md`
10. `./init.md.d/workflow-done.md`

## Core Operating Rules

- Do not invent requirements that conflict with the project specification.
- Do not add libraries, frameworks, services, or tooling without justification.
- Inspect existing code before changing it.
- Prefer the smallest correct change.
- Preserve working functionality.
- Never hide, suppress, or weaken an error merely to make a test pass.
- Test changes before considering them complete.
- When requirements are ambiguous, use the documented project constraints and
  existing architecture first.
- If a decision would materially change architecture, dependencies, data formats,
  or public behavior, stop and ask the user before proceeding.

## Implementation Principle

Work incrementally:

Understand → Plan → Implement → Test → Review → Report.

Do not treat code generation itself as completion. Completion means the
Definition of Done in `workflow-done.md` has been satisfied.

## Project Brief

The actual application brief is intentionally kept separate from this template.
Populate the project-specific brief in `./init.md.d/project.md` before development.

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
