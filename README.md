
# Android Secret Terminal Magisk Module

**⚠️ Warning:** Installing this module on a device that already includes this terminal as a system app may cause a **bootloop** due to signature conflicts. Use at your own risk.

---

## Description

This Magisk module installs the **hidden Android Terminal** (AOSP version) as a system app.

- Provides access to the secret Android terminal app
- Works via **Magisk overlay (systemless)**
- Minimum supported Android version: **16**
- Requires **root access**

> Note: This module does **not enable KVM**. Devices without hardware virtualization can't use this terminal 

---

## Installation

1. Copy the `terminal.zip` module to your device.
2. Open **Magisk Manager** → Modules → Install from storage.
3. Reboot.
4. Enable it on developer settings
5. enjoy

---

## Permissions Granted

The module ensures that the terminal APK has the following permissions:

- `INTERNET`
- `ACCESS_NETWORK_STATE`
- `MANAGE_EXTERNAL_STORAGE`
- `FOREGROUND_SERVICE`
- `POST_NOTIFICATIONS`

> Microphone permission (`RECORD_AUDIO`) must be granted manually if needed.

---

## Important Notes

- Only install if you **do not have this terminal in your stock firmware**, otherwise a signature conflict occurs.
- Hardware virtualization (KVM/pKVM) is **not included**. AVF VMs will **not run** on devices without virtualization support.
- This module is **systemless** and can be safely removed via Magisk.

---

## License

- The Terminal app source code is part of **AOSP** and licensed under **Apache License 2.0**.
- The prebuilt APK from Google is **proprietary**; this repo does **not redistribute it**.  
- This module only packages the APK for systemless installation and overlays, and includes **module.prop and permission XML**.
- The author is **not responsible** for any device damage or bootloops caused by misuse.

> Safe way to use: clone the repo and provide your own APK from a device running Android 16.

---

## Contribution

Feel free to fork the repository, submit issues, or suggest improvements.
