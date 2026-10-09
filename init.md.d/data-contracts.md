# Data Contracts

Define important data shapes and invariants here.

## Domain Models

### [Model Name]

```text
[TODO]
```

Rules:

- [TODO]

## External APIs

### [API / Service]

Request:

```text
[TODO]
```

Response:

```text
[TODO]
```

Failure responses:

```text
[TODO]
```

## Persistence

Storage format/schema:

```text
[TODO]
```

## Validation

For every externally supplied value, define:

- type
- required/optional status
- allowed range or format
- normalization rules
- failure behavior

## Compatibility

Do not silently change persistent data formats or public API contracts.
If a migration is required, document the migration strategy before implementing it.
