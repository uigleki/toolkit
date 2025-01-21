# toolkit

🛠️ My preferred setup and configurations

## ✨ Features

- Open source first, privacy focused
- Simple yet powerful configurations
- Focus on efficiency and stability
- Based on my [tool selection criteria](criteria/README.md)

## Software List

### Windows

| Category     | Software                                                           |
| ------------ | ------------------------------------------------------------------ |
| Input Method | [小鹤双拼方案](assets/flypy.reg)                                   |
| Main Browser | Firefox                                                            |
| Key Mapping  | PowerToys                                                          |
| Cloud Sync   | MEGA                                                               |
| Compression  | 7-Zip                                                              |
| Dir Encrypt  | Cryptomator                                                        |
| Translation  | Crow Translate                                                     |
| Gaming       | Steam                                                              |
| Uninstaller  | Bulk Crap Uninstaller                                              |
| Dir Sync     | [FreeFileSync](https://freefilesync.org/download.php)              |
| Note Taking  | Anytype                                                            |
| VPN Client   | Cloudflare WARP                                                    |
| Code Editor  | Visual Studio Code                                                 |
| Video Player | mpv.net                                                            |
| Music Player | Clementine                                                         |
| Torrent      | qBittorrent Enhanced                                               |
| Downloader   | Motrix                                                             |
| Font Render  | MacType                                                            |
| Phone Link   | KDEConnect                                                         |
| Optimizer    | [Optimizer](https://github.com/hellzerg/optimizer/releases/latest) |
| Net Speed    | TrafficMonitor                                                     |

### Android

| Category          | Software             |
| ----------------- | -------------------- |
| Live Wallpaper    | Muzei Live Wallpaper |
| File Manager      | MiXplorer            |
| Music Player      | Vinyl Music Player   |
| Weather           | Breezy Weather       |
| 2FA               | Aegis Authenticator  |
| Music Recognition | Shazam               |
| Dictionary        | 欧路词典             |
| Terminal          | Termux               |
| Torrent           | LibreTorrent         |
| Downloader        | Download Navi        |

### Linux

| Category      | Software    |
| ------------- | ----------- |
| English Font  | Ubuntu font |
| High Compress | zstd        |
| Fast Compress | lz4         |
| Shell         | fish        |
| Text Editor   | helix       |
| File Manager  | yazi        |
| IM            | Matrix      |

### Browser Extensions

| Category         | Extension                                                                                  |
| ---------------- | ------------------------------------------------------------------------------------------ |
| Ad Blocking      | [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)             |
| Web Translation  | [Immersive Translate](https://addons.mozilla.org/en-US/firefox/addon/immersive-translate/) |
| Side Translation | [Edge Translate](https://addons.mozilla.org/en-US/firefox/addon/edge_translate/)           |
| Tab Management   | [Tab Stash](https://addons.mozilla.org/en-US/firefox/addon/tab-stash/)                     |
| Steam            | [Augmented Steam](https://addons.mozilla.org/en-US/firefox/addon/augmented-steam/)         |
| Image Search     | [Search by Image](https://addons.mozilla.org/en-US/firefox/addon/search_by_image/)         |

### Optional

| Category        | Software   |
| --------------- | ---------- |
| Office Suite    | OnlyOffice |
| Boot Disk       | Ventoy     |
| Bitmap Editor   | GIMP       |
| Vector Editor   | Inkscape   |
| Paint           | Krita      |
| 3D Modeling     | Blender    |
| Video Transcode | HandBrake  |
| Video Editor    | Kdenlive   |
| Audio Editor    | Audacity   |
| Game Engine     | Godot      |
| Game Assistant  | WeMod      |

## Dev Setup

### Python

```shell
winget install -e --id=astral-sh.uv
uv python install 3.11
```

### VS Code

#### Extensions

General:

1. Tyriar.sort-lines
2. esbenp.prettier-vscode
3. yzhang.markdown-all-in-one
4. supermaven.supermaven

Local Only:

1. PKief.material-icon-theme
2. GitHub.codespaces
3. Continue.continue

Python:

- charliermarsh.ruff
- ms-python.python
- ms-toolsai.jupyter

Miscellaneous:

- jnoortheen.nix-ide
- mads-hartmann.bash-ide-vscode
- mechatroner.rainbow-csv
- mkhl.direnv
- ms-dotnettools.csdevkit
- tamasfe.even-better-toml

#### Settings

Sync Settings Only (avoid syncing other options)

```json
{
  "editor.rulers": [80, 120],
  "extensions.ignoreRecommendations": true,
  "files.eol": "\n",
  "telemetry.telemetryLevel": "off",
  "git.enableSmartCommit": true,
  "git.confirmSync": false,

  "workbench.colorTheme": "Default Light Modern",
  "workbench.iconTheme": "material-icon-theme",
  "continue.enableTabAutocomplete": false,
  "continue.showInlineTip": false,

  "editor.cursorBlinking": "solid",
  "files.autoSave": "afterDelay",
  "files.trimTrailingWhitespace": true,
  "files.insertFinalNewline": true,
  "files.trimFinalNewlines": true,
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll": "explicit",
    "source.organizeImports": "explicit"
  },
  "notebook.formatOnSave.enabled": true,
  "notebook.codeActionsOnSave": {
    "notebook.source.fixAll": "explicit",
    "notebook.source.organizeImports": "explicit"
  },
  "git.autofetch": true,

  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "python.defaultInterpreterPath": ".venv/Scripts/python",
  "jupyter.askForKernelRestart": false,
  "[python]": {
    "editor.defaultFormatter": "charliermarsh.ruff"
  },
  "[toml]": {
    "editor.defaultFormatter": "tamasfe.even-better-toml"
  },
  "[csharp]": {
    "editor.defaultFormatter": "ms-dotnettools.csharp"
  }
}
```

## App Config

### mpv.conf

```conf
vo=gpu-next
hwdec=auto-safe

slang=chs,sc,zh
alang=jpn,ja,jp
sub-auto=fuzzy

fullscreen=yes
idle=once
save-position-on-quit=yes
```

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

## 📄 License

[AGPL-3.0](LICENSE)
