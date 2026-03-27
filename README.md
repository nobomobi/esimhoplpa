# eSIMHopLPA

A modern cross-platform eSIM Local Profile Assistant (LPA) application built with **Kotlin** and **Compose Desktop**.

## Download

**Current status:** prebuilt installers are **Windows only**, with an **English** user interface. There is no macOS / Linux installer or localized (non-English) UI package in this repository yet.

**Recommended:** get the latest MSI from [**Releases**](https://github.com/nobomobi/esimhoplpa/releases).

- Download **`eSIMHopLPA-1.0.0.msi`** (or newer) from the release assets.
- Double-click the MSI and follow the setup wizard.
- Ensure **PC/SC** is available on Windows (**WinSCard**).

The same MSI is in the repository root (**Git LFS**); clone only if you need the file via Git.

## Features

- **Profile management**: View, enable, disable, delete, and download eSIM profiles
- **Notification management**: Process and remove eSIM notifications
- **Chip information**: View eUICC details including EID and certificate issuers
- **Cross-platform (from source)**: The codebase can run on Windows, macOS, and Linux when built locally; **published installers are currently Windows (English UI) only**
- **Modern UI**: Jetpack Compose Desktop and Material 3

## Requirements

### Running from source (developers)

- **JDK 21** or later
- **lpac** binary (automatically bundled or manually placed in `~/.esimhoplpa/<platform>/`)
- **PC/SC** (smart card access)
  - **Windows**: Built-in (**WinSCard**)
  - **macOS**: Built-in
  - **Linux**: Install `pcscd` and `pcsc-lite`

### End users (Windows MSI, English UI)

- **Windows 10/11** (64-bit recommended)
- UI: **English** (no other localized installer is published yet)
- **eSIM-capable** hardware exposed via **PC/SC** (see your device documentation)
- No separate **JDK** install required for the packaged installer (runtime is bundled)

## Repository layout

- **`eSIMHopLPA-1.0.0.msi`** — Windows installer, English UI (Git LFS)
- **`.gitattributes`** — Git LFS pointer rules for large binaries

## License

Specify your license here (e.g. MIT, Apache-2.0) if applicable.
