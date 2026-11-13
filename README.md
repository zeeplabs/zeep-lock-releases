<div align="center">

# Zeep Lock

**A free, simple password manager for Mac — with a separate vault for each part of your life.**

[🇧🇷 Português](README.pt-BR.md) · **English**

[**⬇️ Download the latest version**](../../releases/latest)

</div>

<!-- Screenshots: add images to a `screenshots/` folder and reference them here, for example:
![Zeep Lock](screenshots/main-window.png)
-->

## What is Zeep Lock?

Most password managers dump everything in one place. **Zeep Lock keeps what shouldn't mix apart**: your work passwords in one vault, your personal ones in another, a client project in a third. Each vault is independent, and you create as many as you need.

It is **free**, runs **locally on your Mac**, and has **no servers of its own**.

## Features

- 🗂️ **Vaults** — separate work, personal and project passwords.
- 🔑 **Credentials** — title, username, URL, password, notes and tags; favorites and search by title and URL.
- 🎲 **Password generator** — choose the length and the character types, and see how strong each password is.
- 🛡️ **Security audit** — spot weak passwords.
- 📥 **Import and export** — import a CSV or JSON file exported by another password manager, and export an **encrypted** backup protected by a password you choose.
- 👆 **Touch ID** — optional, to unlock without typing your master password.
- ⏱️ **Auto-lock** — after inactivity, and always when your Mac sleeps, the screen locks or the screen saver starts.
- 📋 **Clipboard care** — copied passwords are cleared after a while and are kept out of the Universal Clipboard.
- ☁️ **iCloud sync (beta, optional)** — see below.

## Security

- Your data is **encrypted on your Mac**. Passwords, usernames, notes, titles, URLs, tags and vault names are all encrypted — not only the password.
- A random 256-bit key encrypts your data (AES-GCM). That key is protected by a key derived from your **master password** (PBKDF2-HMAC-SHA256, 600,000 iterations).
- **Your master password cannot be recovered.** If you forget it, the only way forward is to erase the data on that Mac and start over. Keep it somewhere safe.
- Zeep Lock has **no account and no server**. Nothing is sent to Zeep Labs.

> Zeep Lock has not had an independent security audit. Judge it accordingly, and keep an encrypted backup of what matters.

## iCloud sync (beta)

Sync is **optional and off by default**. When you turn it on, it keeps your iCloud vaults in sync between your Macs through **your own iCloud account**, with the data already encrypted. A vault can also stay on this Mac only.

It is a **beta**: it has not been validated across several Macs yet. Keep an encrypted backup (Settings ▸ Import & Export), and don't treat sync as your only copy.

## Download and install

1. Open [**Releases**](../../releases/latest) and download the `.dmg` file.
2. Open it and **drag Zeep Lock to Applications**.
3. Open Zeep Lock from Launchpad or Spotlight and create your master password.

The app is **signed and notarized by Apple**. The `SHA-256` of each file is in the release notes if you want to check your download.

**Requirements:** macOS 26.5 or later.

## Updates

Zeep Lock **updates itself**: when a new version is out, it tells you and you choose whether to install it. To do that, the app checks this project's update feed once a day, which reveals your IP address and the app version to the host (GitHub). Nothing else is sent. Every update is verified with a cryptographic signature before it is installed.

## Frequently asked questions

**I forgot my master password. Can you recover my passwords?**
No. There is no recovery, by design: nobody but you can read your data. On the lock screen, "Forgot your master password?" lets you erase the data on that Mac and start again. If you kept an encrypted export, you can import it afterwards.

**Where are my passwords stored?**
On your Mac, encrypted. If you turn on iCloud sync, an encrypted copy is also stored in your own iCloud account.

**Is it really free?**
Yes.

**Does it work on iPhone or Windows?**
Not for now. Zeep Lock is a Mac app.

## Feedback and bugs

Open an [issue](../../issues) in this repository. **Never include passwords, your master password or backup files** in an issue.

## About

This repository only holds the published versions and the update feed. The source code is not public.

© Zeep Tecnologia. All rights reserved. Made by [Zeep Labs](https://github.com/zeeplabs).
