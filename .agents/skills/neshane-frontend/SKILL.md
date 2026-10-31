---
name: neshane-frontend
description: Implement or extend Neshane V3 frontend features while preserving framework-neutral feature, state, and integration boundaries.
---

# Neshane frontend

Apply to frontend feature, navigation, state, or API-integration implementation. Read `../../../AGENTS.md`, `../../../architecture/governance-baseline.md`, and the relevant local standards. Confirm the Task ID and approved framework/protocol decisions; if missing, report them rather than selecting tools. Build logically isolated feature modules against a shared Design System; do not introduce independent Micro-Frontend deployment without a new approved decision. Prevent cycles, separate server/local/session state, map transport DTOs where meaning differs, use contract-first compatible evolution, and treat the resource-owning Backend service as final authorization authority. Add only structures required by the feature.

Deliver the smallest authorized implementation, required executable tests, configuration/contract notes, decision gaps, applicable readiness-evidence status, and the required Persian report. Follow `AGENTS.md` for approved-toolchain dependency resolution, build/test and isolated local application/container validation. Do not infer a framework decision, production deployment, publishing, push or Security Sign-off.

