# Part3D Bridge

Cross-platform desktop helper that lets **Part3D on iPad** send STL files directly to your slicer. No cables, no cloud, your iPad finds the Bridge on your local network and you send models with one tap.

## Download

**[Go to Releases →](https://github.com/part3d-app/part3d-bridge/releases)** and download the build for your platform:

| Platform    | Notes                                                                  |
| ----------- | ---------------------------------------------------------------------- |
| **macOS**   | Apple Silicon (M-series) only. macOS 10.15 (Catalina) through Sequoia. |
| **Windows** | Coming Soon.                                                           |
| **Linux**   | Coming Soon.                                                           |

Install and run the Bridge on your computer. It sits in the system tray and waits for Part3D on your iPad to connect.

## Features

- **Auto-discovery** — Your iPad finds the Bridge on the network via mDNS/Bonjour; no manual IP or port setup.
- **One-click import** — Send STL files from Part3D on iPad straight into your slicer.
- **Secure pairing** — First-time device approval with HMAC authentication so only your devices can connect.
- **Smart detection** — The Bridge automatically discovers installed slicers on your system.
- **Lightweight** — Under 10MB binary, under 15MB RAM; runs quietly in the background.
- **System tray** — Stays out of the way with a tray icon; no extra windows.

## Supported slicers

- Orca Slicer
- Bambu Studio
- Creality Print
- **System default** — Any other installed application that can open STL files

## Requirements

- **Part3D** on iPad ( [App Store](https://apps.apple.com/us/app/part3d/id6642710061) ).
- iPad and computer on the same network (Wi‑Fi or wired).
- One of the supported operating systems and slicers above.

## Issues and feature requests

This repository is used for **releases** and for **user feedback**:

- **Bug reports** — [Open an issue](https://github.com/part3d-app/part3d-bridge/issues/new) and describe what went wrong, your OS, and steps to reproduce.
- **Feature requests** — [Open an issue](https://github.com/part3d-app/part3d-bridge/issues/new) with the “feature request” label (or describe your idea and we’ll label it).

There is no source code in this repo—only this README and the release binaries.

---

For more about Part3D and the Bridge, see [part3d.app](https://part3d.app) and [part3d.app/bridge](https://part3d.app/bridge).
