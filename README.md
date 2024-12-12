# toolkit

🛠️ My preferred setup and configurations

## ✨ Features

- Curated software recommendations for Windows, Android, and Linux
- Browser extensions for enhanced web experience
- Development environment setup guide
- Essential application configurations

## Software List

### Windows

| Category     | Software                                              |
| ------------ | ----------------------------------------------------- |
| Input Method | 小鹤双拼方案                                          |
| Main Browser | Firefox                                               |
| Key Mapping  | PowerToys                                             |
| Cloud Sync   | MEGA                                                  |
| Compression  | 7-Zip                                                 |
| Dir Encrypt  | Cryptomator                                           |
| Translation  | Crow Translate                                        |
| Gaming       | Steam                                                 |
| Uninstaller  | Bulk Crap Uninstaller                                 |
| Dir Sync     | [FreeFileSync](https://freefilesync.org/download.php) |
| Note Taking  | Anytype                                               |
| VPN Client   | Cloudflare WARP                                       |
| Code Editor  | Visual Studio Code                                    |
| Video Player | mpv.net                                               |
| Music Player | Clementine                                            |
| Torrent      | qBittorrent Enhanced                                  |
| Downloader   | Motrix                                                |
| Font Render  | MacType                                               |
| Phone Link   | KDEConnect                                            |

### Android

| Category          | Software             |
| ----------------- | -------------------- |
| Live Wallpaper    | Muzei Live Wallpaper |
| File Manager      | MiXplorer            |
| Music Player      | Vinyl Music Player   |
| Ad Blocking       | 跳过广告             |
| Weather           | Breezy Weather       |
| 2FA               | Aegis Authenticator  |
| VPN Client        | 1.1.1.1 + WARP       |
| Cloud Sync        | MEGA                 |
| Music Recognition | Shazam               |
| Dictionary        | 欧路词典             |
| Terminal          | Termux               |
| Torrent           | LibreTorrent         |
| Downloader        | Download Navi        |

### Linux

| Category        | Software    |
| --------------- | ----------- |
| OS              | NixOS       |
| Version Control | Git         |
| English Font    | Ubuntu font |
| Fast Compress   | lz4         |
| High Compress   | zstd        |
| Text Editor     | helix       |
| File Manager    | yazi        |
| IM              | Matrix      |

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
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
$env:Path = "C:\Users\uigle\.cargo\bin;$env:Path"
uv python install 3.12
```

### VS Code

#### Extensions

General:

1. esbenp.prettier-vscode
2. Tyriar.sort-lines
3. yzhang.markdown-all-in-one
4. supermaven.supermaven

Local Only:

1. PKief.material-icon-theme
2. GitHub.codespaces
3. Continue.continue

Python:

1. ms-python.python
2. ms-toolsai.jupyter
3. charliermarsh.ruff

Miscellaneous:

1. mechatroner.rainbow-csv
2. tamasfe.even-better-toml
3. ms-dotnettools.csdevkit

#### Settings

Sync Settings Only (avoid syncing other options)

```json
{
  "editor.rulers": [80, 120],
  "extensions.ignoreRecommendations": true,
  "files.eol": "\n",
  "telemetry.telemetryLevel": "off",
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

## 📄 License

[AGPL-3.0](LICENSE)