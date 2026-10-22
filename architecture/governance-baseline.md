# Frontend governance baseline

- Shared reference: `NESHANE-V3-GOV-P00-000A`.
- Repository role: independent, framework-neutral Frontend.
- Root source when the workspace is present: `../../architecture/governance-synchronization.md` and approved Root ADRs/standards.
- This local file is a sufficient fallback when Root is unavailable; it does not approve any framework or unresolved technical choice.

Required invariants: feature boundaries, no Backend implementation coupling, versioned integration contracts, DTO/model separation where useful, server/local/session state separation, Backend-owned authorization, untrusted tenant input, no browser secrets, semantic design tokens, responsive accessible UI, and RTL/Persian support.

If Root is missing, continue only where local standards and an approved Task ID are sufficient. If the reference is outdated, a decision is absent, or guidance conflicts, report the exact issue and pause only affected architecture-sensitive work. Update this reference only through an authorized governance-alignment task.

