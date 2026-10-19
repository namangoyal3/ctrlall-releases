# ctrl+all releases

This repository holds the downloads and the update feed for [ctrl+all](https://ctrlall.app). It holds no source code.

## Requirements

- A Mac with macOS 14.5 or later. Apple silicon and Intel both work.
- At least one agent CLI, signed in, such as Claude Code or Codex.
- Your own account with that agent's vendor. ctrl+all does not supply model access.

## Install

1. Open the [latest release](https://github.com/namangoyal3/ctrlall-releases/releases/latest).
2. Download `ctrl+all-<version>.dmg` and `READ-ME-FIRST.txt`.
3. Check the checksum. `READ-ME-FIRST.txt` tells you how.
4. Open the DMG and drag ctrl+all to Applications.
5. Open ctrl+all from Applications.

Since version 1.0.0 the app is signed with an Apple Developer ID and notarized by Apple, so macOS opens it without a warning.

**If macOS warns you that it cannot open the app, or says it is damaged, do not override the warning.** It means the file is not the one we published. Delete it and write to support@ctrlall.app.

If you ran a beta build before 1.0.0, it cannot update itself to 1.0.0: the release key changed with the first production release. Download the 1.0.0 DMG, quit the beta, and drag the new app over the old one. Your chats and settings stay. macOS then asks once more for the microphone and for Files & Folders access, because the signing identity changed too.

## Updates

Always open ctrl+all from the Applications folder. A copy that runs from the DMG cannot update.

The app checks this repository for a newer version. When one is ready, the sidebar shows "Update available". The app never restarts by itself, so an agent turn in progress is never cut off.

Each update is signed. The app installs only an update that carries a valid signature from the ctrl+all release key.

## Uninstall

Run this command:

```
/Applications/ctrl+all.app/Contents/MacOS/ctrlall uninstall
```

It lists what it will remove and asks you to type `yes`. Then it removes the background agents, stops ctrl+all, and deletes the app. It keeps `~/.ctrlall`.

**Caution: `--purge` cannot be undone.**

To also delete `~/.ctrlall` (chats, keys, and the judge model), add `--purge`.

## Help

Write to support@ctrlall.app. For a problem, run `ctrlall diagnose` first and attach the file it writes to your Desktop:

```
/Applications/ctrl+all.app/Contents/MacOS/ctrlall diagnose
```

## Terms

Read `BETA-TERMS.md` in the release before you use ctrl+all. It says what the beta protects, what it does not, and what leaves your Mac.
