<div align="center">

# WinVora

**Keep Windows updated, clean, and easy to understand.**

[![Latest Version](https://img.shields.io/github/v/release/WinVora/WinVora-Releases?style=for-the-badge&color=7c5cff&label=Version)](https://github.com/WinVora/WinVora-Releases/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011-7c5cff?style=for-the-badge&logo=windows11)](#system-requirements)
[![Languages](https://img.shields.io/badge/Languages-English%20%7C%20German-7c5cff?style=for-the-badge)](#)

[**Download WinVora**](https://github.com/WinVora/WinVora-Releases/releases/latest) · [View Source Code](https://github.com/WinVora/WinVora) · [Report an Issue](https://github.com/WinVora/WinVora-Releases/issues)

</div>

WinVora brings essential Windows tools together in one clear and convenient application. Update programs, free up storage, manage startup apps, and review system information without navigating through multiple Windows menus or technical consoles.

## Take a Look

![WinVora Dashboard](screenshots/dashboard.png)

<table>
  <tr>
    <td width="50%"><img src="screenshots/updates.png" alt="Program updates in WinVora"></td>
    <td width="50%"><img src="screenshots/files.png" alt="File cleanup in WinVora"></td>
  </tr>
  <tr>
    <td align="center"><b>Program Updates</b></td>
    <td align="center"><b>File Cleanup</b></td>
  </tr>
</table>

![System information in WinVora](screenshots/system-info.png)

## What WinVora Can Do

### Keep Programs Updated

- Display available updates clearly and install them together
- View the current and new version, size, publisher, and installation source
- Permanently ignore individual programs or update them later
- Follow download, installation, and completion progress in plain language
- Retry individual failed updates
- Suppress restarts where possible and display “Restart required” instead

### Clean Up Windows

- Scan temporary files, system caches, error reports, and browser data
- Show the expected storage gain before anything is deleted
- Clearly identify sensitive areas and protect them with separate warnings
- Select only the categories you want to clean

### Understand Your System

- View CPU, RAM, GPU, drive, network, and Windows information
- Check Microsoft Defender, Firewall, TPM, and Secure Boot separately
- Copy system information or export it as a report
- Review changes detected since the previous scan
- Identify programs or folders that have grown unusually quickly

### Manage Programs

- Search, export, and uninstall installed programs
- Enable or disable startup entries
- Search the update and activity history with clear results
- Export settings, diagnostic reports, and backups

## Installation

1. Open the [**Latest Release**](https://github.com/WinVora/WinVora-Releases/releases/latest) page.
2. Download `WinVora-Setup-x.x.x.exe`.
3. Run the installer and follow the displayed steps.

WinVora does not include advertisements or bundled software. Administrator privileges are requested only when Windows requires them for an action you selected.

> **Windows SmartScreen notice:** The installer is not currently signed with a paid code-signing certificate. Windows may therefore display an “Unknown publisher” warning during the first installation. Only download WinVora from this official repository.

## Security and Privacy

- No telemetry and no sale of personal data
- No hidden background installations
- Cleanup and uninstall operations are initiated by the user
- Technical diagnostic reports can be reviewed before saving
- Personal details are anonymized in support reports
- The source code is publicly available for inspection

### Optional Download Verification

Each installer includes a small `.sha256.txt` file. It is not required for installation, but it allows you to independently verify the downloaded installer:

```powershell
Get-FileHash .\WinVora-Setup-x.x.x.exe -Algorithm SHA256
```

The displayed hash must match the contents of the corresponding `.sha256.txt` file.

## System Requirements

- Windows 10 version 2004 or later, or Windows 11
- 64-bit system
- WinGet for program updates
- Internet connection for update checks and downloads

The remaining areas of WinVora can also be used without an internet connection.

## Help and Feedback

Found a bug or have an idea for WinVora? Create a [GitHub issue](https://github.com/WinVora/WinVora-Releases/issues) and describe what happened in as much detail as possible.

You can also contact me directly by email at [winvoraadmin@gmail.com](mailto:winvoraadmin@gmail.com).

If you enjoy using WinVora and would like to support its continued development, you can support the project on [Ko-fi](https://ko-fi.com/winvora).

---

<div align="center">

Built for Windows users who want to manage their system without unnecessary complexity.

</div>
