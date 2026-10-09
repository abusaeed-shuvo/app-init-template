# Coding Conventions

## General

- Prefer readable code over clever code.
- Keep functions and modules focused.
- Use descriptive names.
- Avoid unnecessary abstraction.
- Avoid duplicated constants and logic.
- Remove temporary debugging code before completion.

## Naming

- Variables: [TODO]
- Functions: [TODO]
- Types/classes: [TODO]
- Files/modules: [TODO]
- Constants: [TODO]

## Formatting

Use the project's formatter/linter when one is defined in `stack.md`.

## Comments

Comments should explain intent, constraints, or non-obvious reasoning.
Do not write comments that merely restate obvious code.

## Error-Prone Code

For code involving parsing, filesystem access, networking, concurrency,
serialization, authentication, or user input:

- validate assumptions
- handle expected failures
- avoid silently ignoring errors
- preserve useful diagnostic information

## Minimal Changes

When fixing a bug, modify the smallest reasonable surface area.
Do not refactor unrelated code during a focused fix.
