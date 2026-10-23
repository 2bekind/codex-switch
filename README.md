<div align="center">

<img src="assets/Icon.png" width="76" alt="Codex Switch icon">

# Codex Switch

Simple account switcher for Codex

[![Latest release](https://img.shields.io/github/v/release/2bekind/codex-switch?style=flat-square&color=ffffff&labelColor=161616)](https://github.com/2bekind/codex-switch/releases/latest) ![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-ffffff?style=flat-square&labelColor=161616) ![Architecture](https://img.shields.io/badge/builds-x64%20%2B%20x86-ffffff?style=flat-square&labelColor=161616) [![Boosty](https://img.shields.io/badge/Boosty-support-F15F2C?style=flat-square&labelColor=161616)](https://boosty.to/swixhub)

**[Download x64](https://github.com/2bekind/codex-switch/releases/latest/download/Codex.Switch.exe)** · **[Download x86](https://github.com/2bekind/codex-switch/releases/latest/download/Codex.Switch.x86.exe)** · [Releases](https://github.com/2bekind/codex-switch/releases) · [Usage](#usage)

</div>

## Preview

<table>
  <tr>
    <td align="center"><img src="Preview.png" width="350" alt="Account list with subscription days, remaining Codex limits and reset times"></td>
    <td align="center"><img src="assets/Light.png" width="350" alt="Light theme with demo accounts"></td>
  </tr>
  <tr>
    <td align="center">Accounts & limits</td>
    <td align="center">Light theme</td>
  </tr>
</table>

Screenshots use demo accounts.

## Features

- Switch between saved Codex accounts.
- See remaining limits, reset times and subscription days.
- Get Windows notifications when limits recover or a paid subscription ends.
- Keep a name and note for each account.
- Hide email addresses with one click.
- Open profile avatars with a smooth zoom and frosted background.
- OLED black and light themes with a circular transition.
- Russian and English interface, initially selected from Windows settings.
- Smooth scrolling and language transitions.
- Profile avatars and SF Pro when installed.
- Interface icons from coolicons.
- Settings for startup, notifications, appearance and account recovery.
- Optional launch at Windows sign-in, including a quiet start in the tray.

## Usage

1. Download **Codex Switch.exe** (x64, recommended) or **Codex Switch x86.exe** and run it. No installer is needed.
2. Click **Добавить** (Add) and sign in to the account you want to save.
3. Click **Переключить** (Switch) next to an account, then confirm the Codex restart. Finish running tasks before switching.
4. Click the pencil to edit an account's name or note. Click the eye to hide its email.

Click an avatar to view it. Click outside the image or press **Escape** to close it.

Closing the window sends Codex Switch to the system tray. Click its tray icon or launch the EXE again to reopen it. Right-click the tray icon and choose **Выйти** (Exit) to quit completely. Limits and notifications keep working in the tray.

The current Codex account is saved on first launch. **Ctrl+R** refreshes account data and limits. Open the gear at the bottom right for settings. **Other → Restore previous** restores the previous sign-in; **Data** opens the local data folder. **System** controls startup and notifications, and **Appearance** changes the theme.

Requires Windows 10/11 x64, .NET Framework 4.8 and the Microsoft Store version of Codex signed in through ChatGPT. The interface supports Russian and English. Click the globe beside the app title to change the language. Click the moon or sun beside Accounts to change the theme. SF Pro falls back to Segoe UI when unavailable.

Both x64 and x86 executables are tested on 64-bit Windows. The x86 download is an alternative build of the switcher; it does not add support for running Codex on 32-bit Windows. macOS and Linux builds are not available: the current app uses Windows WPF and DPAPI.

## Notifications

Codex Switch keeps running in the system tray when you close its window. Windows notifications continue for:

- Five-hour limit recovery.
- Weekly limit recovery.
- A Plus or Pro subscription changing to Free.

Events are confirmed with fresh server data. The end of a billing period alone does not trigger an expiry notification. Notification history persists across app restarts to prevent duplicates.

Choose which notifications to receive in **Settings → System**, or turn them off entirely.

## Local data

Saved sign-ins are encrypted with Windows DPAPI for the current Windows user and stored in `%LOCALAPPDATA%\CodexSwitch`. Account profiles and limits are requested using each saved sign-in. Account names and notes stay in the local account list.

This repository contains the Windows executable and demo images. It includes no saved accounts, tokens or personal profile data. Source code is not published here.

## Repository stats

[![Stars](https://img.shields.io/github/stars/2bekind/codex-switch?style=flat-square&color=ffffff&labelColor=161616)](https://github.com/2bekind/codex-switch/stargazers) [![Release downloads](https://img.shields.io/github/downloads/2bekind/codex-switch/total?style=flat-square&color=ffffff&labelColor=161616)](https://github.com/2bekind/codex-switch/releases)

The download counter counts release assets. Downloads from the EXE link in the repository are not included.

---

Interface icons: [coolicons by Kryston Schwarze](https://github.com/krystonschwarze/coolicons), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Adapted to WPF vector drawing, resized and recolored; the subscription badge uses a filled background.

Codex Switch is an independent utility and is not affiliated with OpenAI.

---

<div align="center">

### Support Codex Switch

Support development on Boosty.

<a href="https://boosty.to/swixhub"><img src="https://img.shields.io/badge/Support_on_Boosty-F15F2C?style=for-the-badge&logoColor=white" alt="Support Codex Switch on Boosty" height="36"></a>

</div>
