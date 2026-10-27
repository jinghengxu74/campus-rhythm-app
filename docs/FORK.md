# Fork Campus Rhythm To-Do Notes

The Mac sticker source lives at **[campus-rhythm-mini](https://github.com/jinghengxu74/campus-rhythm-mini)** (MIT). You may fork it for personal use, coursework, or your own branded desktop todo.

## Quick start

```sh
git clone https://github.com/YOUR_USER/campus-rhythm-mini.git
cd campus-rhythm-mini
zsh scripts/test.sh
zsh scripts/build.sh
open dist/Campus\ Rhythm\ Mini.app
```

Requires **macOS 13+**, **Apple silicon** for the pre-built zip, and Xcode Command Line Tools.

## If you ship your own build

1. **Change the bundle identifier** in `scripts/build.sh` (`CFBundleIdentifier`) so it does not clash with the official app or overwrite `~/Library/Application Support/CampusRhythmMini/`.
2. **Sign** with your own Apple Development certificate if you distribute to others.
3. **Rename** the `.app` in `build.sh` / marketing if you rebrand — keep support paths documented for your users.
4. **Do not** commit user data, `.env`, or `account-session` files.

## Good fork ideas

- New themes / skins (paper, fonts, compact layout)
- Keyboard shortcuts, export Done list to CSV
- Localization (zh-HK, zh-CN, en)
- Accessibility (VoiceOver labels, larger type)

## Out of scope for casual forks

- Removing consent for optional cloud sync without clear UI
- Bundling analytics or sending task text to third parties without disclosure
- Impersonating the official Campus Rhythm download

## Get help

Open an issue on your fork or on [campus-rhythm-mini/issues](https://github.com/jinghengxu74/campus-rhythm-mini/issues) with macOS version and steps (no private task text).
