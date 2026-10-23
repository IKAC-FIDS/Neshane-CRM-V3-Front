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

- Codex may inspect relevant files, edit source/documentation, and write required test source.
- Codex must not run builds, tests, applications, Docker/containers, deployments, CI/CD, commits, pushes, dependency installation, internet access, or expensive/unrelated validation.
- Do not change Git metadata or remotes. Do not claim unexecuted verification passed.
- Implementation reports are in Persian and include changed files, configuration, exact manual build/run/deployment/verification commands, and limitations.
- Documentation-only reports must not invent those commands; report documents, approval gaps, manual review, conflicts, and the next authorized task.

