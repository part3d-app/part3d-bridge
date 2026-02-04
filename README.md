# Part3D Bridge

Cross-platform desktop helper that lets **Part3D on iPad** send STL files directly to your slicer. No cables, no cloud, your iPad finds the Bridge on your local network and you send models with one tap.

## Download

**[Go to Releases →](https://github.com/part3d-app/part3d-bridge/releases)** and download the build for your platform:

| Platform    | Notes                                                                  |
| ----------- | ---------------------------------------------------------------------- |
| **macOS**   | Apple Silicon (M-series) only. macOS 10.15 (Catalina) through Sequoia. |
| **Windows** | Coming Soon.                                                           |
| **Linux**   | **AppImage**. Requires GTK and `libappindicator` (see Linux notes).    |

Install and run the Bridge on your computer. It sits in the system tray and waits for Part3D on your iPad to connect.

## Features

- **Auto-discovery** — Your iPad finds the Bridge on the network via mDNS/Bonjour; no manual IP or port setup.
- **One-click import** — Send STL files from Part3D on iPad straight into your slicer.
- **Secure pairing** — First-time device approval with HMAC authentication so only your devices can connect.
- **Smart detection (macOS/Windows)** — The Bridge automatically discovers supported slicers installed on your system.
- **Linux behavior** — On Linux, the Bridge does **not** auto-detect slicers; it opens the **default STL handler** configured by your desktop environment (KDE, GNOME, etc.).
- **Lightweight** — Under 10MB binary, under 15MB RAM; runs quietly in the background.
- **System tray** — Stays out of the way with a tray icon; no extra windows.

## Supported slicers

On **macOS and Windows**, the Bridge auto-detects common slicers (and can also fall back to your system default STL app).

- Orca Slicer
- Bambu Studio
- Creality Print
- **System default** — Any other installed application that can open STL files

On **Linux**, the Bridge opens whatever your desktop environment has configured as the default app for `.stl` files:

## Requirements

- **Part3D** on iPad ( [App Store](https://apps.apple.com/us/app/part3d/id6642710061) ).
- iPad and computer on the same network (Wi‑Fi or wired).
- One of the supported operating systems and slicers above.
- **Linux (AppImage)**: GTK and `libappindicator` are required (see Linux notes below for install commands).

## Linux (AppImage)

The Linux build is distributed as an **AppImage**. If the app doesn’t start or the tray icon doesn’t appear, you’re likely missing runtime dependencies.

### Install dependencies

**Fedora / RPM-based (dnf)**:

```bash
sudo dnf install gtk3 libappindicator-gtk3
```

**Ubuntu / Debian-based (apt)**:

```bash
sudo apt update
# Ubuntu 24.04+ (recommended)
sudo apt install libgtk-3-0 libayatana-appindicator3-1
# Older Ubuntu/Debian
sudo apt install libgtk-3-0 libappindicator3-1
```

## Issues and feature requests

This repository is used for **releases** and for **user feedback**:

- **Bug reports** — [Open an issue](https://github.com/part3d-app/part3d-bridge/issues/new) and describe what went wrong, your OS, and steps to reproduce.
- **Feature requests** — [Open an issue](https://github.com/part3d-app/part3d-bridge/issues/new) with the “feature request” label (or describe your idea and we’ll label it).

There is no source code in this repo—only this README and the release binaries.

---

For more about Part3D and the Bridge, see [part3d.app](https://part3d.app) and [part3d.app/bridge](https://part3d.app/bridge).
