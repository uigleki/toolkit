# toolkit

My preferred setup and configurations

## Features

- Open source first, privacy focused
- Simple yet powerful configurations
- Focus on efficiency and stability
- Based on my [tool selection criteria](docs/criteria.md)

## Software List

### Windows

| Category     | Software                 |
| ------------ | ------------------------ |
| Cloud Sync   | MEGA                     |
| Code Editor  | Visual Studio Code       |
| Compression  | 7-Zip                    |
| Dir Encrypt  | Cryptomator              |
| Dir Sync     | [FreeFileSync][freefile] |
| Downloader   | Motrix                   |
| Font Render  | [MacType][mactype]       |
| Gaming       | Steam                    |
| Image Viewer | ImageGlass               |
| Input Method | [小鹤双拼方案][flypy]    |
| Key Mapping  | PowerToys                |
| Main Browser | Firefox                  |
| Mesh Network | Tailscale                |
| Music Player | Clementine               |
| Net Speed    | TrafficMonitor           |
| Note Taking  | Anytype                  |
| Optimizer    | [Optimizer][optimizer]   |
| Phone Link   | KDEConnect               |
| Sandbox      | Sandboxie Plus           |
| Torrent      | qBittorrent Enhanced     |
| Translation  | Crow Translate           |
| Uninstaller  | Bulk Crap Uninstaller    |
| VPN Client   | Cloudflare WARP          |
| Video Player | mpv.net                  |
| WSL          | [Nixos][nixos]           |

[freefile]: https://freefilesync.org/download.php
[mactype]: https://github.com/snowie2000/mactype/releases/latest
[flypy]: configs/flypy.reg
[optimizer]: https://github.com/hellzerg/optimizer/releases/latest
[nixos]: https://github.com/nix-community/NixOS-WSL/releases/latest

### Android

| Category          | Software                 |
| ----------------- | ------------------------ |
| 2FA               | Aegis Authenticator      |
| Dictionary        | 欧路词典                 |
| Downloader        | Download Navi            |
| FOSS              | F-Droid                  |
| File Manager      | MiXplorer                |
| Live Wallpaper    | Muzei Live Wallpaper     |
| Music Player      | Gramophone               |
| Music Recognition | Shazam                   |
| Torrent           | LibreTorrent             |
| Weather           | [Breezy Weather][breezy] |

[breezy]: https://breezy-weather.github.io/fdroid-repo/fdroid/repo

### Linux

| Category      | Software    |
| ------------- | ----------- |
| Compress Fast | lz4         |
| Compress High | zstd        |
| English Font  | Ubuntu font |
| File Manager  | yazi        |
| Shell         | fish        |
| Text Editor   | helix       |

### Browser Extensions

| Category         | Extension                      |
| ---------------- | ------------------------------ |
| Ad Blocking      | [uBlock Origin][ublock]        |
| Steam            | [Augmented Steam][augsteam]    |
| Tab Management   | [Tab Stash][tabstash]          |
| Translation Side | [Edge Translate][edgetrans]    |
| Translation Web  | [Immersive Translate][imtrans] |

[ublock]: https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/
[augsteam]: https://addons.mozilla.org/en-US/firefox/addon/augmented-steam/
[tabstash]: https://addons.mozilla.org/en-US/firefox/addon/tab-stash/
[edgetrans]: https://addons.mozilla.org/en-US/firefox/addon/edge_translate/
[imtrans]: https://addons.mozilla.org/en-US/firefox/addon/immersive-translate/

### Optional

| Category        | Software   |
| --------------- | ---------- |
| 3D Modeling     | Blender    |
| Audio Editor    | Audacity   |
| Bitmap Editor   | GIMP       |
| Boot Disk       | Ventoy     |
| Game Assistant  | WeMod      |
| Game Engine     | Godot      |
| Office Suite    | OnlyOffice |
| Paint           | Krita      |
| Vector Editor   | Inkscape   |
| Video Editor    | Kdenlive   |
| Video Transcode | HandBrake  |

## Dev Setup

### Python

```powershell
powershell -c "irm astral.sh/uv/install.ps1 | iex"
uv python install 3.12
```

### Code OSS Extensions

General:

- DavidAnson.vscode-markdownlint
- Tyriar.sort-lines
- prettier.prettier-vscode
- usernamehw.errorlens
- yzhang.markdown-all-in-one

Nix:

- jnoortheen.nix-ide
- mkhl.direnv

Python:

- charliermarsh.ruff
- ms-python.python
- ms-toolsai.jupyter

Miscellaneous:

- Dart-Code.flutter
- golang.go
- mads-hartmann.bash-ide-vscode
- mechatroner.rainbow-csv
- ms-vscode.powershell
- muhammad-sammy.csharp
- rust-lang.rust-analyzer
- tamasfe.even-better-toml

## App Config

- [flypy.reg](configs/flypy.reg) - 小鹤双拼输入法方案
- [mpv.conf](configs/mpv.conf) - mpv media player settings
- [vscode-settings.json](configs/vscode-settings.json) - Code OSS settings

### Windows Optimizer

- General
  - System
    - Optimize Performance
    - Disable Error Reporting
    - Disable Sticky Keys
  - Apps
    - All except Mozilla
  - Privacy
- Windows 11
  - Windows Update
  - Privacy
    - All except Enhance Privacy

## License

[CC BY-SA 4.0](LICENSE)
