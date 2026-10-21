# Campus Rhythm — User guide

[Open the web app](https://campus-rhythm-one.vercel.app) · [Project overview](README.md)

Updated 21 October 2026. The web app is a prototype. iOS screenshots show a development build, not a downloadable App Store release.

## 1. Choose a workspace

Use Google or email sign-in for an account workspace. Follow the verification or recovery prompts shown by the app. Where offered, Local mode lets you use the planner on that browser/device without account synchronization.

New account users are directed toward importing existing commitments. Goals and rest preferences can be configured afterward. A separate demo workspace contains fictional examples; it is not your account plan.

Account synchronization is implemented, but this guide does not imply that every browser, device and email-provider combination has passed acceptance. Confirm important work is present after reopening before relying on a second device.

## 2. Import a small set first

Open **Import** or the student import guide.

| Source | What to provide | What to check |
| --- | --- | --- |
| Supported Canvas calendar | The private feed URL obtained from your institution's Canvas calendar. | Deadlines, dates and any unspecified times. The hosted importer restricts accepted feed hosts. |
| Class timetable | An `.ics` export, such as an HKUST Timetable Planner export. | Course/section, recurrence, holiday exclusions and timezone. A preview export does not establish enrollment. |
| Other class/event calendars | A supported `.ics` file. | Import warnings and the dates/times shown in preview. Not every external feed or ICS extension is supported. |

Preview → select items → review → confirm. Start with a few recognizable records. Cancel if the source or timezone looks wrong.

Imports are snapshots. Changes made later in Canvas or another calendar are not automatically fetched. Reimporting the same records supports deduplication; inspect the preview before confirming. Batch removal and restore are available for supported imported records, with newer edits preserved where supported.

Keep feed URLs private. Never paste one into a GitHub issue or public screenshot.

## 3. Read Today and Calendar

**Today** highlights a recommended next step and its explanation. It may instead ask you to protect a saved rest window. A missing assessment weight is unverified, not zero.

**Calendar** provides month, week and day views of the same commitments. Check the all-day/due section as well as timed events. A date-only deadline has no verified clock time; scheduling preparation does not change the original due date.

The desktop Today screen is shown below. Its titles are examples visible in the owner's supplied screenshot.

![Desktop Today interface](assets/web-today-2026-10-21.png)

## 4. Add work and ask Rhythm

1. Add a task with a title, due date and estimated remaining effort.
2. Ask **Rhythm** to help plan an existing task, or request a draft for a new task. Supply missing dates or duration when asked.
3. Review the proposed dates, fixed commitments, rest windows and workload.
4. Edit or confirm the supported change. A conversation is not a saved commitment until you confirm it.

Example request: “Help me plan my existing Engineering assignment before Friday; I still need two hours.” This is an example, not a guarantee that every wording will be interpreted correctly. Check the draft.

Cloud AI requires an authenticated account and an available service. It interprets the message; local rules perform planning checks. If unavailable, follow the local-planner option shown by the app. Do not include private information in an AI message that you do not want sent to the provider.

## 5. Record progress and review

- Use **Done** when work is actually finished. Scheduled minutes alone do not establish completion.
- Record progress/actual effort where offered, and check the completed-task history.
- Use **Undo completion** or the relevant undo control for supported recent changes. Do not assume arbitrary historical changes can always be reversed.
- Open **Weekly review** to inspect recorded work and remaining tasks. Missing records are not evidence of inactivity or poor wellbeing.

## 6. Native development features

iOS development builds include widget, Live Activity and notification integrations. Availability depends on the installed build and system permissions. Notifications are opt-in; review quiet hours and title-privacy settings. iOS controls widget refresh timing.

Apple Health is an optional, read-only native connection for sleep, steps and exercise minutes. It is unavailable on the web. Completing the permission dialogue does not prove that every reading was granted. Missing readings remain unknown. Real physical-iPhone readings and the full native journey still need acceptance.

## 7. Common problems

| What you see | What to do |
| --- | --- |
| An import is rejected | Follow the source-specific guide. Check whether the host/file format is supported. Do not share the private URL publicly. |
| The source calendar changed | Obtain a fresh export/feed snapshot and review a reimport; continuous external sync is not connected. |
| A deadline has no time | Keep it date-only unless you can verify the time. Choose preparation time separately. |
| AI is unavailable or reaches a limit | Use the local planner or try later. A failed AI response should not create a plan change. |
| A suggestion is wrong | Edit/cancel the draft before saving. Include expected versus actual behavior in a sanitized report. |
| A change is missing on another device | Check the account and synchronization status; resolve any conflict rather than assuming a successful save. |
| You cannot find the iOS download | No public App Store/TestFlight distribution is claimed. Use the web prototype. |
| Apple Health is empty | Check the supported native build and device permissions; do not treat empty data as a zero reading. |

## Feedback

Use [GitHub Issues](https://github.com/jinghengxu74/campus-rhythm-app/issues) for ordinary product bugs and documentation corrections, or the optional [survey](https://forms.gle/8ue3LXgotZLrxNzX9) for usability feedback. Provide the screen, steps, expected result, actual result and browser/device. Remove names, emails, feed tokens and private task details.

[Privacy boundaries](docs/PRIVACY.md) · [Current verification](docs/EVALUATION.md) · [Roadmap](docs/ROADMAP.md)
