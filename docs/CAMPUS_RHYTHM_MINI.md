# Campus Rhythm Mini · macOS to-do sticker

**Campus Rhythm Mini** (friendly name: **Campus Resume Sticker**) is a free, open-source floating note for macOS. It sits in the menu bar or folds into a small circle so you can capture tasks, mark them done, and skim the last seven days of completions without opening a full planner.

The in-app menu title is **Rhythm Note**; the product family name is **Campus Rhythm**.

## Download (Apple silicon, macOS 13+)

1. Download **[Campus-Rhythm-Mini-macOS-arm64-v0.9.37.zip](../assets/downloads/Campus-Rhythm-Mini-macOS-arm64-v0.9.37.zip)** from this showcase repository.
2. Unzip and move **Campus Rhythm Mini.app** to Applications (or run from the folder).
3. On first open, macOS may warn that the app is from an unidentified developer. Open **System Settings → Privacy & Security** and choose **Open Anyway**, or right-click the app → **Open** once.

Builds are **ad-hoc signed**, not notarized. They are intended for personal use and classroom demos.

## Build from source

Source code: **[github.com/jinghengxu74/campus-rhythm-mini](https://github.com/jinghengxu74/campus-rhythm-mini)**

```sh
git clone https://github.com/jinghengxu74/campus-rhythm-mini.git
cd campus-rhythm-mini
zsh scripts/test.sh
zsh scripts/build.sh
open dist/Campus\ Rhythm\ Mini.app
```

Requires Xcode Command Line Tools on Apple silicon Mac.

## What it does

| Area | Behavior |
| --- | --- |
| **To-do / Pending / Completed / Events** | Daily intentions beside your calendar day; undated inbox; completion history with a swipeable seven-day chart. |
| **Windows** | Pin, resize, fold to a draggable circle, open another day in a second window. |
| **Appearance** | Light/dark glass, paper tint, fonts, per-task highlights. |
| **Account** | Optional sign-in to the same Campus Rhythm notebook as [web Daily notes](https://campus-rhythm-one.vercel.app/notes). Local notes stay separate until you import them. |

Data is stored locally under `~/Library/Application Support/CampusRhythmMini/`. Do not commit that folder or session files.

## Privacy

The Mac sticker does not read Apple Health. Calendar events for the Events tab come from your connected Campus Rhythm account. See the main [privacy notes](PRIVACY.md) for web and account boundaries.

## Support the project

If this sticker saves you a daily glance at what matters, please **star**:

- [campus-rhythm-app](https://github.com/jinghengxu74/campus-rhythm-app) (product showcase)
- [campus-rhythm-mini](https://github.com/jinghengxu74/campus-rhythm-mini) (open-source Mac app)

Report Mac-specific issues on the [mini repository](https://github.com/jinghengxu74/campus-rhythm-mini/issues) with screenshots and macOS version; remove personal task text when possible.
