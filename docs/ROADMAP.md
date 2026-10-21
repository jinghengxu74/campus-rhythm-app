# Roadmap and acceptance criteria

[Overview](../README.md) · [Current evidence](EVALUATION.md)

Updated 21 October 2026. Priorities express intended work, not release commitments. No dates are promised.

| Priority | Work | What would count as done |
| --- | --- | --- |
| Now | Unassisted first-run web journey | New students complete sign-up → import preview → confirm → plan → Done/Undo → review; blockers and assistance are recorded. |
| Now | Simplify the first page and import flow | Observe a specific usability blocker, change it, and retest the same task; publish what improved and what did not. |
| Now | Account and recovery acceptance | Verify refresh, sign-out/in, recovery, second-device persistence and user isolation on hosted services. |
| Now | Physical-iPhone acceptance | Install a current native build and verify HealthKit permissions/readings, widgets, Live Activities, reminders and title privacy separately. |
| Now | Broader source lint cleanup | Resolve the repository-wide lint findings and document the supported check scopes. |
| Next | More seamless scheduling | Draft a task and feasible sessions from a natural-language request; handle ambiguity, conflicts, confirmation and undo without silent writes. |
| Next | Feedback-led pilot | Use an unassisted five-student rehearsal as a proposed gate, audit 30 planning scenarios, then consider a 20–30 student pilot. Report recruitment and results separately. |
| Later | Health-aware scheduling | Test whether consented, locally derived health context usefully constrains suggestions; preserve unknown readings and data boundaries. |
| Later | Shared-time discovery | Validate a limited availability-sharing flow, privacy controls and revocation before promising a complete social planner. |
| Later | Continuous external connections | Design provider authorization, refresh, duplicates, conflicts and revocation before claiming live Canvas/Outlook sync. |

The pilot numbers above are proposed targets. They are not completed sessions, enrolled participants or evidence of outcomes.

## How progress will be reported

For each meaningful release, record the problem, implementation, environment, checks run, user acceptance and remaining limits. Keep Designed, Implemented, Deployed, Live-tested and Planned distinct. A feature leaves the roadmap only when its stated acceptance criteria have evidence.
