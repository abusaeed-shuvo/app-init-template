# Workflow and Definition of Done

## Standard Workflow

### 1. Understand

Read the relevant project instructions and inspect the existing implementation.

### 2. Plan

Identify:

- affected files
- required changes
- dependencies
- tests
- possible failure modes

For small changes, keep the plan proportional to the task.

### 3. Implement

Make incremental changes.
Avoid unrelated refactoring.

### 4. Verify

Run relevant tests and validation commands.

### 5. Review

Check:

- correctness
- error handling
- security
- regressions
- consistency with architecture
- unnecessary complexity
- documentation impact

### 6. Report

Summarize:

- what changed
- what was tested
- any known limitations
- any decisions requiring user input

## Definition of Done

A feature/bug fix is complete only when applicable items are satisfied:

- [ ] Requirement implemented
- [ ] Existing behavior preserved
- [ ] Error cases handled
- [ ] Relevant tests added/updated
- [ ] Tests pass
- [ ] Linter/formatter passes when applicable
- [ ] Build/package validation passes
- [ ] No debug code remains
- [ ] Security implications checked
- [ ] Documentation/contracts updated if necessary
- [ ] No unrelated changes introduced

## Git Safety

- Do not destroy user changes.
- Do not use destructive git commands without explicit approval.
- Do not commit secrets.
- Keep changes logically focused.

## Final Rule

Never claim a task is complete based solely on code being written.
Completion requires verification.
