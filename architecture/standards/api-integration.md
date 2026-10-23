# API integration

- Design integration contracts before implementation and prefer backward-compatible additions.
- Route remote calls through a centralized, replaceable client boundary with consistent base configuration, correlation, cancellation, timeouts, serialization, and error translation.
- Use typed versioned contracts where practical; do not import Backend implementation or persistence types.
- Map transport DTOs to feature/domain/view models when frontend meaning or lifecycle differs.
- Handle authentication/session credentials through an approved secure mechanism. Tenant values sent by the client are selectors only.
- Normalize safe user-facing errors while retaining correlation details for diagnostics. Never display raw stack traces, secrets, or sensitive payloads.
- Define cancellation for superseded navigation/search and bounded timeouts for remote operations. Retry only safe/idempotent requests under an approved policy.
- Detect incompatible contract versions and fail visibly with a recovery/update path.
- A breaking API/session contract requires a new version, coexistence window, explicit deprecation, consumer migration plan and removal criteria; do not assume simultaneous Backend/Frontend deployment.

REST versus GraphQL, code generation, base client library, retry policy, and credential transport remain unapproved.

