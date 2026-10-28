# Install Campus Rhythm To-Do Notes

Latest checked release: v0.9.58 (29 October 2026).

[Download for Apple silicon](https://github.com/jinghengxu74/campus-rhythm-mini/releases/latest/download/Rhythm-Note-macOS-arm64.zip) · [Release history](https://github.com/jinghengxu74/campus-rhythm-mini/releases/latest)

Requires an Apple silicon Mac (M1 or newer) and macOS 13 or later. The supplied binary does not support Intel Macs. No Xcode, developer account or paid subscription is needed for local notes.

1. Download the ZIP from this repository's official release, then unzip it.
2. Move Campus Rhythm Mini.app to Applications. Quit an older running copy first after saving any draft.
3. Open it. The legacy application filename differs from the product name, Campus Rhythm To-Do Notes.
4. Local notes work without signing in. Account synchronization is optional; use your own Campus Rhythm account. Apple Calendar requires its separate system permission.

## Apple cannot verify this app

This release is ad-hoc signed, not Developer ID signed or notarized. The warning is not by itself a malware detection, and it is not proof that the app is safe. Re-downloading the same release does not remove the notarization warning.

Only if you trust the publisher and intend to test this build, follow [Apple's instructions](https://support.apple.com/en-gb/102445): after attempting to open the app, open System Settings → Privacy & Security and review the blocked application and Open Anyway option. This is a user decision. Do not disable Gatekeeper, remove quarantine attributes, or bypass a malware/damaged-app warning. Managed Macs may prohibit exceptions; use the [web planner](https://campus-rhythm-one.vercel.app) instead.

## Verify the release

For v0.9.58 the published ZIP SHA-256 is:

`774e62f431aba237f2388b125e71bde0c1469223450e645e22e83259f5e82420`

A matching hash establishes identical bytes, not absence of malware. Independent antivirus and complete dynamic security testing are not claimed.

## Updates and feedback

Version 0.9.58 adds an in-app notice for newer releases while the app runs. It opens the release page; it does not automatically install updates. Older versions require a manual update once.

Report macOS version, Apple/Intel chip, app version, exact warning and reproduction steps through GitHub Issues. Remove personal task/calendar information from screenshots. Avoid important-only copies of tasks during early testing; keep your own backup.
