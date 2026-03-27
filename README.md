# eSIMHopLPA

A modern cross-platform eSIM Local Profile Assistant (LPA) application built with **Kotlin** and **Compose Desktop**.

## Download

**Current status:** prebuilt installers are **Windows only**, with a **Simplified Chinese** user interface. There is no macOS / Linux installer or English UI package in this repository yet.

**Recommended:** get the latest MSI from [**Releases**](https://github.com/nobomobi/esimhoplpa/releases).

- Download **`eSIMHopLPA-1.0.0.msi`** (or newer) from the release assets.
- 简体中文界面：双击 MSI，按安装向导完成安装。
- Ensure **PC/SC** is available on Windows (**WinSCard**).

The same MSI is in the repository root (**Git LFS**); clone only if you need the file via Git.

## Features

- **Profile management**: View, enable, disable, delete, and download eSIM profiles
- **Notification management**: Process and remove eSIM notifications
- **Chip information**: View eUICC details including EID and certificate issuers
- **Cross-platform (from source)**: The codebase can run on Windows, macOS, and Linux when built locally; **published installers are currently Windows (简体中文) only**
- **Modern UI**: Jetpack Compose Desktop and Material 3

## Requirements

### Running from source (developers)

- **JDK 21** or later
- **lpac** binary (automatically bundled or manually placed in `~/.esimhoplpa/<platform>/`)
- **PC/SC** (smart card access)
  - **Windows**: Built-in (**WinSCard**)
  - **macOS**: Built-in
  - **Linux**: Install `pcscd` and `pcsc-lite`

### End users (Windows MSI, 简体中文)

- **Windows 10/11**（建议 64 位）
- UI：**简体中文**（当前无英文或其它语言安装包）
- 需要支持 **eSIM / PC/SC** 的读卡环境（见各硬件说明）
- 安装包已自带运行环境，一般**无需单独安装 JDK**

## Repository layout

- **`eSIMHopLPA-1.0.0.msi`** — Windows 简体中文安装包（Git LFS）
- **`.gitattributes`** — Git LFS pointer rules for large binaries

## License

Specify your license here (e.g. MIT, Apache-2.0) if applicable.
