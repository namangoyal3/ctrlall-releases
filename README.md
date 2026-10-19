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

Apple has not notarized this beta, so macOS stops the app the first time. Do these steps one time:

1. When macOS says it cannot open the app, click **Done**. Do not click Move to Trash.
2. Open **System Settings**, then **Privacy & Security**. Scroll to Security.
3. Click **Open Anyway** next to ctrl+all. Enter your password or use Touch ID.

**Caution: do these steps only for a DMG whose checksum matches the one in `READ-ME-FIRST.txt`.**

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

## Terms

Read `BETA-TERMS.md` in the release before you use ctrl+all. It says what the beta protects, what it does not, and what leaves your Mac.
