# Frontend testing

- Component tests cover behavior, states, accessibility semantics, keyboard interaction, RTL direction, and meaningful variants.
- Integration tests cover feature behavior across components, state, routing, and mocked contract boundaries without reproducing implementation details.
- User-flow tests cover critical entry, decision, action, feedback, recovery, authorization denial, and tenant/session transitions.
- Contract tests or typed fixtures protect integration compatibility; fixtures contain no production secrets or sensitive data.
- Test loading, empty, error, offline/timeout, cancellation, long Persian text, mixed direction, compact layout, and destructive-action safety where applicable.
- Keep tests deterministic and user-observable. A skipped or unexecuted test is not evidence of success.

No test runner, browser automation, component harness, accessibility scanner, screenshot tool, or coverage threshold is approved. Codex may write required test source but must not install or execute test tools under repository policy.

