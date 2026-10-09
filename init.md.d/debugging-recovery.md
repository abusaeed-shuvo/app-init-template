# Debugging and Recovery

When something fails, do not immediately make speculative edits.

## Debugging Procedure

1. Read the complete error.
2. Identify the failing component.
3. Locate the relevant source code.
4. Reproduce the failure when possible.
5. Determine the root cause.
6. Inspect related code and assumptions.
7. Form a hypothesis.
8. Make the smallest appropriate fix.
9. Run the relevant tests.
10. Check for regressions.

## If the First Fix Fails

- Re-read the new error.
- Reassess the root cause.
- Revert unnecessary changes mentally or with safe version-control operations.
- Avoid stacking unrelated patches on top of an incorrect diagnosis.
- Try a different hypothesis based on evidence.

## If Multiple Attempts Fail

Stop escalating random changes.

Report:

- original failure
- what was investigated
- changes attempted
- current failure
- useful logs/output
- what remains uncertain

Ask the user for guidance when further progress requires a product or architectural decision.

## Recovery Rules

- Never delete user data as a debugging shortcut.
- Never reset/revert user work without explicit permission.
- Never disable security mechanisms just to bypass an error.
- Never replace a working subsystem wholesale without first establishing why it is necessary.
