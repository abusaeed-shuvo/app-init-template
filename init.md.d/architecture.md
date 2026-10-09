# Architecture

## Architectural Goal

Keep the application modular, understandable, and easy to modify.

## Structure

Define the project structure here.

```text
[TODO]
```

## Responsibilities

Document where major responsibilities belong.

- UI / presentation: [TODO]
- Business logic: [TODO]
- Data access: [TODO]
- External services: [TODO]
- Configuration: [TODO]
- Utilities: [TODO]
- Tests: [TODO]

## Architectural Rules

- Keep unrelated concerns separated.
- Avoid circular dependencies.
- Do not place business logic inside presentation code unless explicitly justified.
- Do not duplicate core logic across multiple modules.
- Prefer existing abstractions over creating competing ones.
- Do not perform large architectural rewrites to solve local bugs.
- Keep public interfaces stable unless a change is explicitly required.

## Change Boundary

Before making an architectural change, identify:

- affected modules
- reason for the change
- alternatives considered
- migration impact
- tests that must change
