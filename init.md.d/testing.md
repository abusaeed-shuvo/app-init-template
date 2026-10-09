# Testing Rules

Testing is part of implementation, not a final optional step.

## Test Levels

Use the appropriate level for each change:

1. Unit tests for isolated logic.
2. Integration tests for interactions between modules/services.
3. End-to-end tests for important user workflows.
4. Manual verification when automated testing cannot reasonably cover behavior.

## Required Checks

After meaningful changes:

- run the relevant tests
- run the formatter/linter if configured
- run the build/package check
- verify the changed behavior
- check for regressions in related functionality

## Test Design

Tests should verify:

- normal behavior
- boundary conditions
- invalid input
- expected failures
- regression cases for fixed bugs

## Test Rules

- Do not delete a failing test just because it exposes a bug.
- Do not weaken assertions solely to make tests pass.
- Do not mock away the behavior being tested.
- Keep tests deterministic where practical.

## Completion

A task is not complete while relevant tests are failing unless the user explicitly
accepts the failure.
