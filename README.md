<div align="center">

<img src="assets/Icon.png" width="76" alt="Codex Switch icon">

# Codex Switch

Simple account switcher for Codex

[![Latest release](https://img.shields.io/github/v/release/2bekind/codex-switch?style=flat-square&color=ffffff&labelColor=161616)](https://github.com/2bekind/codex-switch/releases/latest) ![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-ffffff?style=flat-square&labelColor=161616) ![Architecture](https://img.shields.io/badge/architecture-x64-ffffff?style=flat-square&labelColor=161616)

**[Download EXE](https://github.com/2bekind/codex-switch/raw/refs/heads/main/Codex%20Switch.exe)** · [Releases](https://github.com/2bekind/codex-switch/releases) · [Usage](#usage)

</div>

## Preview

<table>
  <tr>
    <td align="center"><img src="Preview.png" width="350" alt="Account list with subscription days, remaining Codex limits and reset times"></td>
    <td align="center"><img src="assets/Notes.png" width="350" alt="Account name and note editor"></td>
  </tr>
  <tr>
    <td align="center">Accounts & limits</td>
    <td align="center">Names & notes</td>
  </tr>
</table>

Screenshots use demo accounts.

## Features

- Switch between saved Codex accounts.
- See remaining limits, reset times and subscription days.
- Get Windows notifications when limits recover or a paid subscription ends.
- Keep a name and note for each account.
- Hide email addresses with one click.
- OLED black interface, profile avatars and SF Pro when installed.

## Usage

1. Download **Codex Switch.exe** and run it. No installer is needed.
2. Click **Добавить** (Add) and sign in to the account you want to save.
3. Click **Переключить** (Switch) next to an account, then confirm the Codex restart. Finish running tasks before switching.
4. Click the pencil to edit an account's name or note. Click the eye to hide its email.

The current Codex account is saved on first launch. **Ctrl+R** refreshes account data and limits. **Вернуть предыдущий** restores the previous sign-in.

Requires Windows 10/11 x64, .NET Framework 4.8 and the Microsoft Store version of Codex signed in through ChatGPT. The interface is currently in Russian. SF Pro falls back to Segoe UI when unavailable.

## Notifications

Keep Codex Switch open or minimized to receive Windows notifications for:

- Five-hour limit recovery.
- Weekly limit recovery.
- A Plus or Pro subscription changing to Free.

Events are confirmed with fresh server data. The end of a billing period alone does not trigger an expiry notification. Notification history persists across app restarts to prevent duplicates.

## Local data

Saved sign-ins are encrypted with Windows DPAPI for the current Windows user and stored in `%LOCALAPPDATA%\CodexSwitch`. Account profiles and limits are requested using each saved sign-in. Account names and notes stay in the local account list.

This repository contains the Windows executable and demo images. It includes no saved accounts, tokens or personal profile data. Source code is not published here.

## Repository stats

[![Stars](https://img.shields.io/github/stars/2bekind/codex-switch?style=flat-square&color=ffffff&labelColor=161616)](https://github.com/2bekind/codex-switch/stargazers) [![Release downloads](https://img.shields.io/github/downloads/2bekind/codex-switch/total?style=flat-square&color=ffffff&labelColor=161616)](https://github.com/2bekind/codex-switch/releases)

The download counter counts release assets. Downloads from the EXE link in the repository are not included.

---

Codex Switch is an independent utility and is not affiliated with OpenAI.
