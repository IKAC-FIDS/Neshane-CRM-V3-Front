# Neshane V3 Frontend instructions

## Authority and baseline

- Work only on the explicitly requested Task ID and do not modify unrelated files.
- This is an independent Frontend repository. It must remain independently developable and understandable.
- Read `architecture/governance-baseline.md` and the relevant files under `architecture/standards/` before work.
- The recorded references are architecture `NESHANE-V3-ARCH-P00-002` and governance `NESHANE-V3-GOV-P00-000A`. Root architecture and approved V3 ADRs are authoritative when available.
- If Root guidance is missing, use the local baseline without inventing decisions. If it is stale or conflicts with Root, report the mismatch and stop affected architecture-sensitive work until authorized resolution.
- No frontend framework, API protocol, state library, UI kit, styling system, test framework, or authentication library is approved yet.

## Frontend invariants

- Use modular, feature-oriented architecture with logically isolated feature modules, explicit public surfaces, and no circular dependencies.
- Use a shared Design System for semantic tokens, reusable accessible components and interaction patterns. Independent Micro-Frontend deployment is not initially required.
- Do not couple to Backend implementation details. Use approved, versioned contracts and map API DTOs to frontend models where needed.
- Use contract-first integration and controlled compatibility; breaking contracts require a new version, coexistence, deprecation and consumer migration planning.
- Separate server, local UI, and session state. Shared state requires demonstrated cross-feature need.
- Frontend permissions are UX controls only; Backend resource-owning services make final authorization decisions under shared Policy Governance. Never embed secrets or trust tenant/session state as proof.
- Use semantic design tokens, accessible reusable components, responsive layouts, and first-class RTL/Persian behavior without premature generic abstractions.
- Architecture, Implementation and Production Readiness are separate evidence gates; unexecuted checks are not evidence.

## Local skills and execution policy

Use the smallest relevant set: `.agents/skills/neshane-frontend`, `neshane-ui`, and `neshane-frontend-review`.

- An explicit Frontend development Task authorizes ordinary in-scope source/documentation edits, configured local tooling, builds, tests, application runs, debugging, defect fixes and repeated validation without per-command approval. This permission does not select a framework/tool that remains architecturally unresolved.
- Resolve pinned or controlled dependencies only from repository-declared approved official HTTPS registries with normal TLS validation. Preserve lockfiles and integrity controls where supported; reject untrusted mirrors, arbitrary executable installers and disabled checks, and record material dependency changes.
- Task-owned local applications and Docker containers may run for isolated smoke/integration testing using trusted base images with approved provenance/integrity controls, localhost binding by default, no production credentials/customer data, no privileged/host-network mode, no sensitive host/Docker-socket mounts, bounded resources, and cleanup limited to Task-created disposable resources.
- Do not disable tests or weaken security/architecture checks. Commit only when the Task explicitly authorizes it. Deployment, publishing, CI/CD, push, remote infrastructure mutation, production access and release require separate authorization; do not change Git metadata/remotes without explicit scope.
- Do not claim unexecuted verification passed or treat local evidence as Security Sign-off or Production Readiness.
- Implementation reports are in Persian and include changed files, configuration, exact manual build/run/deployment/verification commands, and limitations.
- Documentation-only reports must not invent those commands; report documents, approval gaps, manual review, conflicts, and the next authorized task.

