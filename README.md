# WinVora

A modern, Windows 11-style system utility app — live hardware monitoring, storage cleanup, app updates, and program management in one clean, fast tool.

Built solo in a week with WinUI 3 / Windows App SDK. No telemetry, no bundled junk, no "one-click optimize everything" snake oil — just the tools, and you decide what to run.

![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-blue)
![Status](https://img.shields.io/badge/status-early--stage-orange)
![Language](https://img.shields.io/badge/UI-English%20%2F%20Deutsch-lightgrey)


## Features

### 📊 Live Dashboard
- Real-time CPU, RAM, and GPU usage
- CPU/GPU temperature (via LibreHardwareMonitor, where supported by your hardware)
- Mini history charts for CPU/RAM/GPU (last 30 samples)
- Storage overview, installed program count, last cleanup time, available Winget updates — all at a glance
- Recent activity log (cleanups, updates, uninstalls)

### 🧹 Storage Cleanup
- 20 categories: temp files, browser cache, thumbnail cache, Windows Update cache, old Windows.old installs, crash dumps, error reports, and more
- Per-category or bulk cleanup, with size shown before you delete anything
- Categories that need admin rights are clearly marked and handled via a single UAC prompt, not one per item

### 📦 App Updates (Winget)
- Scans installed packages via `winget` and shows available updates
- Select which apps to update, or update everything at once
- Live progress per package

### 🗑 Program Uninstaller
- Full list of installed programs with real extracted icons
- Search/filter, one-click uninstall

### 🎨 Design
- Windows 11 Fluent Design: Mica backdrop, rounded cards, soft shadows, accent-colored hover states
- Dark and light mode
- Fully bilingual: **English and German**, switchable anytime in Settings (also asked on first launch)

### 🔄 Auto-Update
- Checks GitHub Releases in the background
- One click to download and install the latest version — WinVora restarts itself automatically

---

## Installation

1. Go to [Releases](../../releases) and download the latest `WinVoraSetup-x.x.x.exe`
2. Run the installer

> **⚠️ Windows SmartScreen warning:** This installer isn't code-signed (that costs money I haven't put into this hobby project yet), so Windows may show a blue "Windows protected your PC" screen on first run. Click **"More info" → "Run anyway"** to continue. This is expected and not a sign of anything malicious — the source is right here in this org if you want to check for yourself.

### Requirements
- Windows 10 (version 2004 / build 19041) or Windows 11
- 64-bit (x64)

---

## Why no admin rights by default?

WinVora runs as a normal user. A handful of storage categories (like `Windows.old` or upgrade logs) are owned by `TrustedInstaller` and genuinely need elevation — for those specific items only, WinVora asks for a single UAC confirmation instead of requiring the whole app to run as admin all the time.

## Known limitations

- GPU usage and temperature depend on [LibreHardwareMonitor](https://github.com/LibreHardwareMonitor/LibreHardwareMonitor) support for your specific hardware. If your GPU isn't supported, those fields will honestly show "Not available" instead of a fake number.
- Some sensors (especially temperatures) may only report correctly when run elevated, depending on your system.

---

## Feedback & Bug Reports

This is a very young project (started this week) built by one person, so things *will* break. If they do:

- Open an [Issue](../../issues) with what happened, your Windows version, and (if possible) the log file from `%LOCALAPPDATA%\WinVora\log.txt`
- Or just comment wherever you found this — I read everything

Feature suggestions are welcome too.

## Roadmap (ideas, not promises)

- Autostart manager (see/disable startup programs, estimated impact)
- Scheduled/automatic cleanup scans
- System tray support
- Keyboard shortcuts

---

## Built with

- [WinUI 3](https://learn.microsoft.com/windows/apps/winui/winui3/) / Windows App SDK
- [CommunityToolkit.WinUI](https://github.com/CommunityToolkit/Windows)
- [LibreHardwareMonitor](https://github.com/LibreHardwareMonitor/LibreHardwareMonitor) — GPU/temperature sensor readings
- Winget (Windows Package Manager) for app updates

## Support

If you'd like to support the project: [ko-fi.com/winvora](https://ko-fi.com/winvora)

---

*This is an independent hobby project and is not affiliated with Microsoft.*
