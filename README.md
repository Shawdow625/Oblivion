<div align="center">

# OBLIVION
### An independent Minecraft: Java Edition launcher for Windows

**Modern desktop experience · Legitimate Microsoft sign-in · Customizable Minecraft instances**

**Status: In active development — public release not yet available**

</div>

---

## About Oblivion

**Oblivion** is an independently developed Windows desktop launcher for **Minecraft: Java Edition**. It aims to provide a modern launcher interface, Minecraft instance management, and secure sign-in for players who own the game.

The desktop application is built with **Tauri, Rust, React, and TypeScript**. This repository is a public information page for the project; the application's source code is not currently published here.

## Planned and developing functionality

- **Microsoft account sign-in:** System-browser OAuth 2.0 authorization-code flow with PKCE.
- **Official authentication chain:** Xbox Live, XSTS, and Minecraft Services authentication.
- **Ownership validation:** Check legitimate Minecraft: Java Edition entitlements before authenticated launches.
- **Account management:** Manage multiple signed-in Minecraft accounts and select the desired account.
- **Instance management:** Organize Minecraft versions and launcher configurations.
- **Desktop-first interface:** A responsive Windows launcher experience.

Some functionality is still being implemented or tested and may change before release.

## Microsoft / Minecraft AppID review

Oblivion is requesting authorization for its **own Microsoft application registration** to interact with official Minecraft Services APIs. The project does not use another launcher's client ID.

| Detail | Value |
| --- | --- |
| Application name | Oblivion |
| Microsoft Application (client) ID | `babf65d7-c2fc-4875-a4ce-35dab75db9db` |
| Platform | Windows desktop |
| Client type | Public/native application |
| Redirect URI | `http://localhost/oauth/callback` |
| Authentication | Microsoft OAuth 2.0 + PKCE → Xbox Live → XSTS → Minecraft Services |
| Approval status | Not yet approved; AppID review submission being prepared |

The launcher is designed to use a system browser for Microsoft sign-in, preserve token confidentiality through native application storage, and verify game ownership with Minecraft Services. It **does not bypass login, ownership, licensing, or platform safety checks**.

## Availability

Oblivion is currently under active development and does not yet offer a general public download. A release, if made available, will be announced through this repository.

## Disclaimer

Oblivion is an **unofficial, independently developed third-party launcher**. It is **not affiliated with, approved by, or endorsed by Mojang Studios or Microsoft**. Minecraft, Mojang, Xbox, and Microsoft names and trademarks belong to their respective owners.

Use of the launcher is subject to applicable Minecraft and Microsoft terms, license requirements, and usage guidelines.
