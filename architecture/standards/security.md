# Frontend security

- Frontend visibility and permission checks improve UX but never authorize an operation. Shared Policy Governance may provide policy inputs, but the resource-owning Backend service makes and enforces the final resource/action decision; Sovereign policy authority is local.
- Treat route parameters, browser storage, API payloads, tenant selections, and all user-controlled values as untrusted.
- Never embed secrets, private keys, privileged service credentials, or sensitive environment values in browser bundles or source.
- Keep tenant selection and session state explicitly separated and re-established through approved Backend contracts. Use approved credential handling with secure expiry, logout, renewal, tenant/session transition and cross-tab behavior. Do not invent token storage rules before the identity decision.
- Avoid unsafe HTML execution and untrusted URL/navigation behavior. Escape/render untrusted content through framework-safe mechanisms once selected.
- Minimize sensitive data in client state, telemetry, logs, errors, caches, and persistence. Clear security-sensitive state on logout or tenant/session change.
- Security failures must provide safe recovery without exposing resource existence or policy internals.

Authentication library, token/session storage, CSP, browser persistence, telemetry/redaction, and threat-model details require approval.

