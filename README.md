<p align="center">
  <img src="logo.svg" width="96" alt="Brim logo" />
</p>

<h1 align="center">Brim</h1>

<p align="center">
  <b>A Dynamic Island, a vertical taskbar, a launcher and a desktop toolkit for Windows 10 and 11.</b><br />
  Local-first: no account, no cloud, no telemetry.
</p>

This repository only hosts Brim's installers. Brim itself is proprietary software, and its source code is private.

## Download

Get the newest `Brim_<version>_x64-setup.exe` from **[Releases](https://github.com/KaustubhChowdhury/brim-releases/releases/latest)**.

Each release also has a `SHA256SUMS.txt`, so you can check that the download is intact:

```powershell
Get-FileHash .\Brim_1.30.1_x64-setup.exe -Algorithm SHA256
```

The hash should match the line for that file in `SHA256SUMS.txt`.

## Installing

1. Run the installer. Windows SmartScreen may warn you because the installer isn't code-signed yet: choose **More info → Run anyway**.
2. Accept the licence, choose to install for yourself or for all users, and finish.

**Requirements:**
- Windows 10 1809 or later, or Windows 11, on x64.
- The WebView2 runtime. Windows 11 includes it; on Windows 10 the installer adds it if needed.

## Updating

Brim updates itself: Settings → About → **Updates** → **Update to vX**. It downloads the installer from here, checks it against `SHA256SUMS.txt`, closes, updates in place (your settings and data stay), and opens again.

## Licence

Copyright © 2026 Kaustubh Chowdhury. All rights reserved. See [LICENSE.txt](LICENSE.txt).
Brim includes open-source components under their own licences; they're listed in the THIRD-PARTY-NOTICES.txt installed with the app.
