<p align="center">
  <a href="https://ctrlall.app"><img src="https://ctrlall.app/assets/og.png" alt="ctrl+all: coding agents, finally multiplayer. Product preview with a phone chat." width="960" /></a>
</p>

<h1 align="center">Multiplayer for humans + coding agents.</h1>

<p align="center">One shared flow. Your team. Your agents. Your phones.</p>

<p align="center"><a href="https://ctrlall.app"><strong>Download for Mac at ctrlall.app →</strong></a></p>

ctrl+all brings your teammates into the same coding-agent session. Run Claude Code or Codex on your Mac. Pair each teammate's phone, give them a role, and watch, steer and answer supported approvals together. Use the agent accounts you already pay for.

## Stop handing over prompts. Start working together.

Remote teamwork should not mean another call, a screen share, and a long explanation of what you told the agent. Keep the work in one shared session instead.

| Watch together | Steer together | Approve with a role |
| :--- | :--- | :--- |
| Follow the same chat, tool output and diffs from paired phones. | Send a task, redirect a running turn, or queue the next message. | Owners and operators answer supported requests. Viewers follow without controlling the agent. |

**Your Mac runs the agents. Your phones are windows into the work.** The Mac must stay awake and online. ctrl+all does not provide model access or add per-token charges.

## Try it with a teammate

1. **Get the Mac app from [ctrlall.app](https://ctrlall.app).** The website is the download starting point.
2. **Start one real task.** Choose a project and an available Claude Code or Codex installation. Sign in to your agent vendor if needed.
3. **Pair your phone.** Scan the QR code, open the link in your browser, and approve the device on the Mac.
4. **Bring someone in.** Give a teammate their own paired phone and a role. Watch the same work, send guidance, and try a supported approval.

You need macOS 14.5 or later, an Apple silicon or Intel Mac, and an installed agent CLI with your own vendor account. The phone client runs in a browser; scanning the QR does not install a native app. On iPhone, adding it to the Home Screen is a separate Safari action.

## What's available, and what isn't

| Available today | Not a promise in the public app |
| :--- | :--- |
| Shared chats through individually paired phones; owner, operator and viewer roles | One-click public session join links and live presence |
| Claude Code and Codex; other engine adapters are experimental | Identical support and permissions across every engine |
| Phone chat, steering, and supported permission/question cards | Automatic Google-verified names on every prompt |
| Goals, routines, project memory, and git review from paired devices | A public native iPhone + Apple Watch companion download |

The hero above is a product preview, not evidence that every planned feature is released. Features on the main development branch can arrive before a signed public app update. Permission mode, device role and engine support still apply; multiplayer does not bypass them.

## Help us test the shared flow

Try one useful task, then repeat it with a teammate. Tell us:

- Could both people find and follow the same work?
- Was it clear who could send a task or approve a request?
- Where did pairing, steering or reconnecting become confusing?
- What forced you back to a call or screen share?

Send feedback to [support@ctrlall.app](mailto:support@ctrlall.app). Never include keys, tokens, private prompts or source code in a public report.

## Install safely

Download only through [ctrlall.app](https://ctrlall.app), then open the disk image and drag ctrl+all to Applications. Open it from Applications, not from the disk image. Follow the verification instructions supplied with the download.

Production releases from version 1.0.0 use Apple Developer ID signing and notarization. If macOS warns that the app is damaged or cannot be verified, do not bypass the warning. Delete the download and contact [support@ctrlall.app](mailto:support@ctrlall.app).

If you still use a beta from before 1.0.0, get the current installer through the website, quit the beta and replace the app in Applications. Chats and settings stay; macOS may ask for permissions again because the signing identity changed.

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

To also delete `~/.ctrlall` (chats and keys), add `--purge`.

## Help

Write to support@ctrlall.app. For a problem, run `ctrlall diagnose` first and attach the file it writes to your Desktop:

```
/Applications/ctrl+all.app/Contents/MacOS/ctrlall diagnose
```

## Terms

Read `BETA-TERMS.md` in the release before you use ctrl+all. It says what the beta protects, what it does not, and what leaves your Mac.

## About this repository

This repository stores release artifacts and the update feed. It is not the product download starting point. For installation and current product information, go to [ctrlall.app](https://ctrlall.app).
