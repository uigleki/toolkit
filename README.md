# toolkit

My preferred setup and configurations

## Features

- Open source first, privacy focused
- Simple yet powerful configurations
- Focus on efficiency and stability
- Based on my [tool selection criteria](criteria/README.md)

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
[flypy]: assets/flypy.reg
[optimizer]: https://github.com/hellzerg/optimizer/releases/latest
[nixos]: https://github.com/nix-community/NixOS-WSL/releases/latest

### Android

| Category          | Software             |
| ----------------- | -------------------- |
| 2FA               | Aegis Authenticator  |
| Dictionary        | 欧路词典             |
| Downloader        | Download Navi        |
| File Manager      | MiXplorer            |
| Live Wallpaper    | Muzei Live Wallpaper |
| Music Player      | Gramophone           |
| Music Recognition | Shazam               |
| Torrent           | LibreTorrent         |
| Weather           | Breezy Weather       |

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

```shell
winget install -e --id=astral-sh.uv
uv python install 3.12
```

### VS Code

#### Extensions

General:

1. tyriar.sort-lines
2. esbenp.prettier-vscode
3. yzhang.markdown-all-in-one
4. supermaven.supermaven
5. github.copilot

Local Only:

1. pkief.material-icon-theme

Python:

- charliermarsh.ruff
- ms-python.python
- ms-toolsai.jupyter

Miscellaneous:

- anthropic.claude-code
- github.codespaces
- golang.go
- jnoortheen.nix-ide
- mads-hartmann.bash-ide-vscode
- mechatroner.rainbow-csv
- mkhl.direnv
- ms-dotnettools.csdevkit
- ms-vscode-remote.remote-wsl
- rust-lang.rust-analyzer
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

  "workbench.colorTheme": "Solarized Light",
  "workbench.iconTheme": "material-icon-theme",

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
  "python.defaultInterpreterPath": ".\\.venv\\Scripts\\python.exe",
  "jupyter.askForKernelRestart": false,
  "[python]": {
    "editor.defaultFormatter": "charliermarsh.ruff"
  },
  "[rust]": {
    "editor.defaultFormatter": "rust-lang.rust-analyzer"
  },
  "[go]": {
    "editor.defaultFormatter": "golang.go"
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

## License

[CC BY-SA 4.0](LICENSE)
