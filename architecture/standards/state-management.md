# State management

- Classify state before implementation: server state is remote cached data; local UI state belongs to the owning view/feature; session state represents authenticated application context.
- Keep state as local as practical. Shared state is justified only when multiple independent consumers require one coherent lifecycle.
- Do not duplicate remote business data into a second client store without an explicit synchronization reason and invalidation policy.
- Treat cached server data as potentially stale. Define refresh, invalidation, optimistic update, rollback, cancellation, and error behavior per use case.
- Derive values instead of storing duplicate computed state. Make ownership and reset/lifetime behavior explicit.
- Tenant and permission values in client state are display/selection context, never proof of authority.

No state-management or server-cache library is approved. Choose one only through an authorized architecture decision based on actual application needs.

