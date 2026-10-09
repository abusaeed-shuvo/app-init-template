# Security and Performance

## Security

- Never hardcode secrets.
- Never commit credentials, API keys, private keys, or tokens.
- Use environment/configuration mechanisms for secrets.
- Validate untrusted input.
- Apply least privilege.
- Do not disable authentication, authorization, TLS, sandboxing, or other security
  controls merely to make development easier.
- Avoid logging sensitive information.
- Treat external files, APIs, and user input as untrusted.

## Dependencies

Prefer maintained, well-understood dependencies.
Avoid adding dependencies for trivial functionality.

## Performance

Do not optimize blindly.

First identify the bottleneck, then optimize the relevant path.

Avoid:

- unnecessary background work
- unbounded memory growth
- uncontrolled polling
- repeated expensive computation
- loading large resources when streaming/lazy loading is practical

## Resource Targets

Define project-specific targets here:

- Startup: [TODO]
- Idle CPU: [TODO]
- Idle memory: [TODO]
- Maximum expected data size: [TODO]

## Compatibility

Define supported:

- OS: [TODO]
- CPU architecture: [TODO]
- runtime versions: [TODO]
- display/platform requirements: [TODO]
