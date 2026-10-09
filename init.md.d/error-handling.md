# Error Handling

Errors must be handled deliberately.

## Categories

Classify failures as appropriate:

- user/input error
- validation error
- configuration error
- filesystem/storage error
- network/external-service error
- dependency/runtime error
- programmer error
- unexpected/system error

## Rules

- Never silently swallow important errors.
- Give users actionable messages when the failure is user-facing.
- Preserve technical details in logs where appropriate.
- Do not expose secrets, credentials, tokens, or sensitive internal data.
- Fail safely when continuing could corrupt state.
- Validate external input before processing it.
- Handle expected failures at the layer that can meaningfully recover from them.

## Recovery

When recovery is possible:

1. Detect the failure.
2. Preserve useful state where safe.
3. Recover or retry according to documented rules.
4. Report failure if recovery does not succeed.

## Retries

Retries must be bounded.

Do not create infinite retry loops or aggressive polling.
Use backoff when repeated external operations are appropriate.

## User-Facing Errors

Messages should say:

- what happened
- whether the user's data/action is affected
- what they can do next

Avoid exposing stack traces or internal implementation details to ordinary users.
