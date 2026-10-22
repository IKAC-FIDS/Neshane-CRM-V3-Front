# Frontend architecture

- Organize code by business feature. Each feature owns its screens, behavior, models, and integration facade; expose a narrow public surface.
- Keep shared UI limited to reusable presentation primitives and patterns. Keep transport/storage/browser integrations behind explicit infrastructure boundaries.
- Dependencies flow from composition/routes to features, and from features to shared UI/infrastructure contracts; features must not form circular dependencies or reach into another feature's internals.
- Do not couple to Backend classes, persistence models, package layout, or deployment topology. Integrate only through approved versioned contracts.
- Keep API DTOs at the integration boundary and map to frontend domain/view models when shape, lifecycle, naming, or presentation needs differ.
- Add abstractions only after a stable repeated need is demonstrated. Do not initialize a framework or architecture skeleton before approval.

Framework, routing, rendering strategy, package layout, localization stack, and generated-contract approach require an approved decision.

