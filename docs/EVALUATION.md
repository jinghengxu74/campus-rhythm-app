# Evaluation and evidence

[Overview](../README.md) · [Architecture](ARCHITECTURE.md) · [Roadmap](ROADMAP.md)

As of **21 October 2026**, application version **1.1.0**, private source commit **`06cb519`**. The public showcase has its own commit history; that history is not the application release history.

## Checks rerun for this documentation update

| Check | Result | What it establishes |
| --- | --- | --- |
| Automated application tests | **201 passed; 0 failed; 0 skipped.** | The current test assertions passed on the inspected local checkout. |
| TypeScript | `tsc --noEmit --incremental false` passed. | Static type checking for that checkout. |
| Standard Expo application lint | Passed using `expo lint -- --cache-location=/tmp/campus-rhythm-showcase-eslint-cache`. | The application's standard Expo lint scope passed; the temporary cache avoids modifying the source checkout. |
| Broader repository ESLint scan | **Did not pass.** | A separate `eslint .` scan reported Node `Buffer` globals, generated server-code lint findings, a PGlite import-parser error and a test import-order warning. This is broader than the standard Expo check and remains unresolved. |
| Live web entry | The production domain loaded the Today interface in an existing browser workspace. | Availability and rendered route content in that session, not independent first-user sign-in acceptance. |
| Screenshot provenance | The latest desktop Today image was provided by the owner for this update. | Interface presentation on 21 October; not evidence of reliability or outcomes. |

The tests cover areas including imports, recurrence/time handling, assistant contracts, planning rules, account/workspace transitions, synchronization, reminders and health summaries. **201 is a test count, not a coverage percentage or a user count.** The source and test suite are private, so readers cannot reproduce these checks by cloning this showcase.

## Earlier maintainer verification

The following records were reviewed rather than repeated during this documentation update:

| Record | Dated evidence | Limit |
| --- | --- | --- |
| Real timetable import regression | 19 October: ten recurring series expanded to 126 occurrences, exactly matching a separate reference calculation including source holiday exclusions. | One HKUST timetable preview export; not proof of enrollment or a broad ICS benchmark. |
| Native file import | 19 October: simulator file-picker import, duplicate detection, batch removal and restore were recorded. | Isolated development workspace and simulator, not a physical iPhone or independent student journey. |
| Native build | 21 October handoff records a Release simulator build/install/launch and Home Screen widget display. | Not App Store/TestFlight distribution; does not verify every native feature. |
| Web deployment | 21 October handoff records a production deployment and alias check. | No new application deployment was performed for this showcase update. |

Raw calendar exports, private account records and internal handoff logs are not included in the public repository. These entries are maintainer-reported evidence, not third-party audits.

## Acceptance still open

- An independent new student completes sign-up, first import, planning, confirmation, Done/Undo and weekly review without assistance.
- Refresh, sign-out/sign-in, recovery, second-device persistence and second-user isolation are verified together against hosted services.
- Physical iPhone HealthKit authorization and real readings, widget refresh behavior, Live Activities and reminders are checked on an installed build.
- Direct notification Done/Snooze actions and Lock Screen accessory behavior receive separate acceptance.
- The wider repository lint findings are triaged and resolved within the source project.
- Pilot feedback is collected, an observed blocker is fixed, and the same journey is retested.

## Product outcomes

No measured improvement in grades, stress, sleep, retention or missed deadlines is claimed. There is no published representative user study, comparative scheduling benchmark, independent security audit or accessibility certification.

The proposed pilot will measure task-level outcomes such as successful first import, time to a confirmed plan, plan correction frequency, follow-through and unwanted alerts. The study design, denominators and limitations should be published with any future results. Proposed sample sizes are recruitment targets, not completed research.

## Reading the status labels

| Label | Meaning |
| --- | --- |
| Designed | A behavior or interaction is specified. |
| Implemented | A code path exists; that alone does not establish deployed behavior. |
| Deployed | A build was published; that alone does not establish an end-to-end journey. |
| Live-tested | A specific journey was exercised on a named environment/date; scope matters. |
| Planned | Work remains and no working implementation is promised. |

This separation is used to keep a visible control, passing test, deployment and actual user acceptance from being treated as the same result.
