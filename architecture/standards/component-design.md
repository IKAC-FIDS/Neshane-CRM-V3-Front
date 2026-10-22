# Component design

- Give components one clear responsibility and a small explicit interface. Prefer composition and meaningful variants over duplicated components or speculative universal wrappers.
- Separate presentation from business behavior when it improves reuse, testing, or clarity; do not split mechanically when a local component is already cohesive.
- Reuse starts with design tokens, then component metrics/variants, then screen composition. Keep raw visual constants out of view bodies when they represent reusable design decisions.
- Use semantic elements, keyboard access, visible focus, accessible names, appropriate target sizes, and understandable status/error announcements.
- Define loading, empty, error, disabled, success, permission-denied, and long-content states where relevant.
- Name components by user-facing role or domain purpose and colocate component-specific tests/styles/assets consistently after the framework layout is approved.

Do not select a component library or create a generic internal design framework without approval and demonstrated need.

