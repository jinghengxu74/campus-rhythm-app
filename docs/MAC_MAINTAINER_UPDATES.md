# How to publish a Mac To-Do Notes update

This is for **you** (the maintainer), not end users. The Mac sticker does **not** pull new binaries from GitHub by itself — users use **… → Check for updates…** and install the zip manually.

## What you cannot do from the app menu

- **No “internal push”** from the top-left menu to every user’s Mac. Apple notarized auto-update would need Sparkle or the App Store; this project ships unsigned zips instead.
- **What the menu does:** **Check for updates…** opens the latest GitHub **Release** page.

## Maintainer workflow

1. **Code** — edit `campus-rhythm-mac` (or the `campus-rhythm-mini` git clone).
2. **Version** — bump `CFBundleShortVersionString` / `CFBundleVersion` in `scripts/build.sh`.
3. **Build** — `zsh scripts/build.sh` → `dist/Rhythm-Note-macOS-arm64.zip`.
4. **Showcase zip** — copy the zip to  
   `campus-rhythm-app/assets/downloads/Campus-Rhythm-To-Do-Notes-macOS-arm64-vX.Y.Z.zip`  
   and update links in `README.md` and `docs/CAMPUS_RHYTHM_TODO_NOTES.md`.
5. **Screenshots** — add PNGs under `campus-rhythm-app/assets/desktop/` and reference them in the doc.
6. **Push source** — commit and push [campus-rhythm-mini](https://github.com/jinghengxu74/campus-rhythm-mini).
7. **Release** — `gh release create vX.Y.Z --repo jinghengxu74/campus-rhythm-mini --title "…" dist/Rhythm-Note-macOS-arm64.zip`.
8. **Push showcase** — commit and push [campus-rhythm-app](https://github.com/jinghengxu74/campus-rhythm-app).

After that, anyone with the app can use **Check for updates…** to reach the new release.
