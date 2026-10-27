# Phase C & D — paste this into a **new Cursor chat** (Campus Rhythm / To-Do Notes folder)

**Do not run C/D in the same thread as heavy code edits.** Copy everything below the line into a new chat when you are ready to launch socially.

---

## Context

- **Product:** Campus Rhythm **To-Do Notes** — local-first macOS desktop sticker (To-do / Pending / **Completed + done chart** / Events). Open source: `github.com/jinghengxu74/campus-rhythm-mini`. Showcase: `github.com/jinghengxu74/campus-rhythm-app`.
- **Goal:** Cold-start **visibility only** for the sticker — not fundraising, not full Campus Rhythm web/iOS push.
- **User:** HK-based student; not profiting; wants a credible developer/profile presence.

## Decisions to make in that chat (agent: advise, don’t auto-spam)

1. **Separate app brand?** Sticker can stay a **sibling product** under Campus Rhythm, or fork brand (e.g. `StickDone`, `DeskTodo`). Compare: Things, Clear, Apple Reminders, Notion, sticky-note apps — our edge = **glass sticker + done week chart + optional sync**.
2. **New GitHub repo?** Already have `campus-rhythm-mini` — only create another repo if rebranding fork; otherwise extend mini repo.
3. **Accounts needed?**
   - **GitHub** — already have showcase + mini.
   - **X (@…)** — new project account vs personal; pin thread with 4 tab screenshots + release link.
   - **Optional:** Product Hunt, r/macapps — later.
4. **Grok / bots:** Draft posts only; human posts manually.

## Phase C tasks (social, week 1)

- [ ] Register X handle; bio = one line + GitHub + “local-first Mac todo sticker”
- [ ] Pin thread: todo-light, pending, completed, events-today images from `campus-rhythm-app/assets/desktop/`
- [ ] 30s screen recording: fold circle → complete task → Completed chart swipe
- [ ] 3 launch posts (Grok drafts → user picks one)
- [ ] One Show HN or r/macapps post (sanitized, no homework titles in screenshots)

## Phase D tasks (fork-friendly, week 2–3)

- [ ] 3× `good first issue` on campus-rhythm-mini
- [ ] README “Built for heavy todo users who wanted a **done list**” story (3 sentences from user)
- [ ] Optional: rename display name in app menu to match To-Do Notes (separate small PR)

## Market snapshot (agent: refresh with web search when executing C/D)

| App | Sticker / float | Done history | Skins | Open source |
| --- | --- | --- | --- | --- |
| Apple Reminders | Widget | Limited | System | No |
| Things | No native sticker | Projects | Minimal | No |
| Notion / Todoist | Web-heavy | Yes | Themes | No |
| **Campus Rhythm To-Do Notes** | **Circle + glass** | **7-day chart** | **Paper/fonts** | **Yes (MIT)** |

## Out of scope for C/D

- China ICP备案 (not operating mainland commercial hosting)
- App Store submission
- Paid tiers

---

*Phase A+B should be done on GitHub before starting C/D.*
