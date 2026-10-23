# Frontend governance baseline

- Architecture reference: `NESHANE-V3-ARCH-P00-002`.
- Governance reference: `NESHANE-V3-GOV-P00-000A`.
- Repository role: independent, framework-neutral Frontend.
- Root source when the workspace is present: `../../architecture/governance-synchronization.md` and approved Root ADRs/standards.
- This local file is a sufficient fallback when Root is unavailable; it does not approve any framework or unresolved technical choice.

Applicable accepted ADRs: ADR-V3-003 (hybrid tenancy), ADR-V3-004 (Sovereign authority), ADR-V3-005 (domain authorization), ADR-V3-008 (contract compatibility), ADR-V3-009 (Frontend), ADR-V3-010 (profile operations), and ADR-V3-012 (readiness).

Required invariants: modular feature-oriented architecture; logically isolated features; shared Design System; no initial Micro-Frontend deployment requirement; no Backend implementation coupling; contract-first compatible integration; DTO/model separation where useful; server/local/session state separation; final Backend domain authorization; untrusted tenant/session input; no browser secrets; responsive accessible UI; and Persian/RTL support.

Architecture approval establishes neither Implementation nor Production Readiness. Framework, rendering, state, UI, authentication and testing technologies remain unresolved until separately approved.

If Root is missing, continue only where local standards and an approved Task ID are sufficient. If either reference is outdated, a decision is absent, or guidance conflicts, report the exact issue and pause only affected architecture-sensitive work. Update these references only through an authorized governance-alignment task.

