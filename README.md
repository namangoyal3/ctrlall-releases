# ctrl+all releases

This repository holds the downloads and the update feed for [ctrl+all](https://ctrlall.app). It holds no source code.

## Install

1. Open the [latest release](https://github.com/namangoyal3/ctrlall-releases/releases/latest).
2. Download `ctrl+all-<version>.dmg`.
3. Open the DMG and drag ctrl+all to Applications.
4. Read `READ-ME-FIRST.txt` in the release before the first launch.

## Updates

The app checks this repository for a newer version. When one is ready, the app shows an update button. The app never restarts by itself, so an agent turn in progress is never cut off.

Each update is signed. The app installs only an update that carries a valid signature from the ctrl+all release key.

## Requirements

- macOS 15 or later on Apple silicon.
- At least one agent CLI, signed in: Claude Code, Codex, Gemini, OpenCode or Cursor.
