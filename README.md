<div align="center">

<img src="assets/icon.png" width="128" height="128" alt="System Management">

# System Management

**Windows PC maintenance and monitoring — in one window**

Sensors and fans, disk cleanup, data transfer, apps and startup, power and recovery.
Every risky action runs only after a review and your confirmation.

[![Latest version](https://img.shields.io/github/v/release/KykMbawrk/system-management-releases?label=version&color=0ea5e9&style=for-the-badge)](https://github.com/KykMbawrk/system-management-releases/releases/latest)
[![Windows 10 / 11](https://img.shields.io/badge/Windows-10%20%2F%2011%20x64-0078D4?style=for-the-badge&logo=windows&logoColor=white)](#-requirements)
[![Downloads](https://img.shields.io/github/downloads/KykMbawrk/system-management-releases/total?label=downloads&color=22c55e&style=for-the-badge)](https://github.com/KykMbawrk/system-management-releases/releases)

### [⬇️ Download the latest version](https://github.com/KykMbawrk/system-management-releases/releases/latest)

<sub>On the release page, use the <b>Download</b> buttons at the top: the <b>installer</b> or the <b>portable</b> version</sub>

</div>

---

## ✨ Features

### 🖥️ System & Monitoring

| | |
|---|---|
| **PC Overview** | CPU, motherboard, graphics card, memory, drives and system status on one screen. Copy or export the report. A readiness check shows whether everything the app needs is in place — and what to do if it isn't. |
| **Sensors** | Temperatures, load, fans, power and network in real time, with 60-second and 5-minute charts. Overheating alerts with a shared threshold or a separate one for each sensor. Export to CSV. |
| **Monitors** | Connected displays with their resolution and refresh rate; the **Identify** button shows which screen is which. New display settings are applied on trial: unless you confirm them, the previous ones come back after a few seconds. |

### 🧹 Cleanup & Storage

| | |
|---|---|
| **Disk Cleanup** | Temporary files, app caches, Windows maintenance and compression. Ready-made **Recommended** and **Maximum cleanup** presets. Scan and review first, then confirm — **nothing is deleted without your consent**. A report for every run. |
| **Schedule** | Automatic cleanup on a schedule, without opening the window, with the task profile you choose. A separate lightweight schedule just for app caches — fine to run every day. |
| **Data Transfer** | Move large folders to another local NTFS drive: a link stays in the old place, so programs notice nothing. Checks before the move, and you can move a folder back at any time. |
| **Explorer** | A file manager with full rights: sees hidden and system items, batch rename, finds the largest files and folders, attributes and ownership. Protected system folders can't be changed — not even by accident. |

### 📦 Apps & Startup

| | |
|---|---|
| **Applications** | Installed programs and their removal together with leftovers in AppData and the registry; built-in Windows apps. |
| **Startup** | Startup programs, scheduled tasks and third-party services. Disabling is a safe action that you can undo at any time. |

### 🌡️ Hardware & Cooling

| | |
|---|---|
| **Cooling** | Motherboard fan control: calibration, **Quiet 30%**, **Balanced 50%** and **Maximum 100%** presets, your own presets and curves, pump marking. Manual control lasts only while the app is open; one button returns control to the board (BIOS/UEFI). Graphics cards are not touched. |
| **Power Management** | Shutdown or restart timer (15–120 minutes), lock, sleep, hibernate, sign out. Power plans, including the hidden **Ultimate Performance**. Restart to BIOS/UEFI, one-time Safe Mode, battery wear report. |

### 🛡️ System & Security

| | |
|---|---|
| **Restore** | Windows restore point, undoing compression, bringing back Windows settings disabled by the cleanup, a journal of completed actions and moving transferred folders back. Each operation runs separately. |
| **Settings** | English and Russian interface; light, dark or system theme; checking for and installing updates, What's New, diagnostics, logs, export and import of settings, PowerShell and Windows Terminal updates, settings reset. |

---

## 🔒 Security and updates

- **Signed updates.** The app verifies every update with the developer's signature (ECDSA P-256) and every file by size and SHA-256. A forged, damaged or outdated update is rejected.
- **Nothing without asking.** The update installer starts only after you confirm it; the portable version never replaces itself.
- **No vulnerable drivers.** The old WinRing0 driver has been removed completely. Full access to motherboard sensors uses the optional, Microsoft-signed [PawnIO](https://pawnio.eu/) driver; without it the app still works and honestly shows which sensors are unavailable instead of false zeros.
- **Protection against mistakes.** System folders are protected from changes, risky actions need a separate confirmation, and most changes can be undone in **Restore**.

---

## 📥 Installation

| | Installer | Portable |
|---|---|---|
| File | `System-Management-Setup-<version>.exe` | `System-Management-Portable-<version>.exe` |
| Setup | Installs into your user profile; desktop shortcut optional | None — a single file you can even carry on a USB stick |
| Updates | Downloaded and installed after your confirmation | Downloaded and verified; you replace the old file yourself |
| First start | Normal | Slower: the app unpacks itself (~1 GB) into `%LOCALAPPDATA%`, after that it starts right away |

> [!NOTE]
> The files are not signed with a publisher certificate yet, so Windows may show "Unknown publisher".
> Click **More info → Run anyway**. The SHA-256 checksum of every file is listed on its release page.

## 💻 Requirements

- Windows 10 or Windows 11, 64-bit
- Administrator rights — the app asks for them at startup (system maintenance needs them)
- About 1 GB of free space for the portable version
- Optional: [PawnIO](https://pawnio.eu/) for motherboard sensors and fans

## ❓ FAQ

<details>
<summary><b>Why does the app ask for administrator rights?</b></summary>

Cleaning system folders and managing services, startup, power and fans require administrator rights — Windows doesn't allow these actions otherwise.
</details>

<details>
<summary><b>Motherboard sensors or fans show as unavailable</b></summary>

Direct access to the motherboard controller needs the PawnIO driver. It's optional: the app neither installs nor removes it. Install PawnIO from its official website and restart the app.
</details>

<details>
<summary><b>How do I update the portable version?</b></summary>

In **Settings → App Update**, click **Check for Updates** and then **Download**. The new version is saved to your **Downloads** folder, already verified. Close the app and replace the old file with the new one — or simply run the new file.
</details>

<details>
<summary><b>Which languages does the app support?</b></summary>

English and Russian. You can switch the language in **Settings**.
</details>

<details>
<summary><b>Where is the source code?</b></summary>

The source code is closed. This repository only publishes ready-made builds and signed update manifests.
</details>
