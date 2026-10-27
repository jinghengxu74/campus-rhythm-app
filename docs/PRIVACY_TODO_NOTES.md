# Privacy · Campus Rhythm To-Do Notes (macOS)

[Full product privacy](PRIVACY.md) covers the web/iOS planner. **This page is only for the Mac desktop sticker.**

**Summary:** Your tasks live on your Mac by default. Nothing is uploaded unless you choose **… → Connect account** and sign in to Campus Rhythm.

## Local by default

| Data | Stored where | Sent to cloud? |
| --- | --- | --- |
| To-do, Pending, Completed, categories, colors, undo history | `~/Library/Application Support/CampusRhythmMini/` | **No** (unless you connect an account and edit synced notes) |
| Window position, appearance per day | Same folder + macOS window autosave | **No** |
| Apple Calendar events (Events tab) | Read on device for display | **Not uploaded** to Campus Rhythm servers through the calendar read path |
| Account session (if connected) | Keychain / local session file on Mac | Tokens used only to reach **your** Campus Rhythm account API |
| Rhythm assistant (optional) | Chat while open | Cloud AI only if you use it while signed in; message text goes through the configured service |

## Optional account sync

- **Disconnected:** Status shows device-only notes. Works offline.
- **Connected:** Notebook can sync with [web Daily notes](https://campus-rhythm-one.vercel.app/notes) on a poll interval (not realtime). You choose **Import local notes** explicitly; IDs are not duplicated blindly.
- **Disconnect:** Returns to local notebook; account cache is isolated per user.

## What we do not do (Mac sticker)

- No sale of task content to advertisers.
- No Apple Health reads on Mac.
- No silent background upload of your full task file.
- No automatic App Store analytics in the unsigned GitHub build (there is no embedded third-party analytics SDK in the open-source tree reviewed for this doc).

## Apple permissions

- **Calendar** — only if you enable Apple Calendar on the Events tab; used to list events for the selected day.
- **Microphone / speech** — only while you use voice capture on a task; review in-app permission prompts.

## Your responsibilities

- Do not commit `~/Library/Application Support/CampusRhythmMini/` or screenshots with real task titles to public repos.
- Treat calendar feed URLs and passwords like credentials.
- Unsigned builds: install only from [official releases](https://github.com/jinghengxu74/campus-rhythm-mini/releases) or your own build.

## Hong Kong / open-source distribution

This is a **free, open-source side project**, not a commercial data broker. If you are in Hong Kong and only use local mode, you are generally processing your own data on your own device. Connecting an account uses the same Campus Rhythm web privacy rules as the hosted app.

*Last reviewed: 27 October 2026. Not legal advice.*
