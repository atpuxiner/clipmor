# Clipmor Usage Guide

Clipmor is a lightweight, low-resource Windows clipboard enhancer.
Clip history supports saving text and images, creating, deleting, keyword search, and pinning; it stores the raw data copied by the system and does not provide editing. A simple built-in todo list supports creating, editing, deleting, keyword search, and pinning.
All data is stored locally in a SQLite database, fully offline, with no network upload and no privacy collection.

[简体中文](README.md) | [English](README.en.md)

## Download

### Microsoft Store (Recommended)

Search `Clipmor` in the Microsoft Store to install:

[Clipmor Microsoft Store](https://apps.microsoft.com/detail/Axiner.Clipmor)

### GitHub Releases

Open the [GitHub Releases page](https://github.com/atpuxiner/clipmor/releases), select the latest version, and download the one that fits your needs:

- **Portable** `Clipmor-portable-vX.X.X.X.zip`: No installation required, just extract and run.
- **Installer** `Clipmor-setup-vX.X.X.X.exe`: One-click installation with an optional desktop shortcut.

## Getting Started

### Portable Version

1. Download and extract the latest portable package (e.g. `Clipmor-portable-vX.X.X.X.zip`) to obtain a file named `clipmor.exe`.
2. Double-click it to run. No installation is required.
3. Copy content as usual, then press `Ctrl+Q` to open the history window.

### Installer Version

1. Download and run the latest installer (e.g. `Clipmor-setup-vX.X.X.X.exe`), then follow the prompts to complete the installation.
2. Launch Clipmor from the Start menu or the desktop shortcut.
3. Copy content as usual, then press `Ctrl+Q` to open the history window.

## Data Storage Location

- **Installer version**: `%LOCALAPPDATA%\Clipmor`
- **Portable version**: The folder containing `clipmor.exe` or `%LOCALAPPDATA%\Clipmor`

Data files:

```text
clipmor.db       # text history
clipmor.imgs/    # image history
```

## Core Features

- Clipboard history: saves text and image records, create, delete, search, pin frequently used content
- Quick search: keyword search to quickly locate history clips
- Pin to top: pin high-frequency content to the top for quick access
- Todo list: built-in simple todos, create, edit, delete, search, pin
- Lightweight background: small footprint, silent tray operation, low performance overhead
- Optional auto-start: disabled by default, enabled manually by the user

## Backup and Migration

- The database is encrypted, so `clipmor.db` cannot simply be copied to another computer or another Windows user.
- Cross-machine migration: Export a CSV on the original computer, then import it on the new computer. For image records, copy the corresponding image files in `clipmor.imgs/` along with the CSV.

## Troubleshooting

- Program does not open: Make sure `clipmor.exe` is not blocked by antivirus software.
- No history visible: Copy some content first, then press `Ctrl+Q` to open the history window.
- History disappeared: Check the data storage location first (see “Data Storage Location” above), then verify that the corresponding `clipmor.db` and `clipmor.imgs/` are still present and have not been deleted.
- Supported systems: Windows 10 / 11.

## License

This project is released under the MIT License (MIT). See [LICENSE](LICENSE)
