# Clean Sweep LIVE

[Download the Clean Sweep LIVE ZIP for Windows 10/11 (64-bit)](https://github.com/DSBMediaCreative/UE5-Tests/releases/download/clean-sweep-live-selected-wardrobes-win64/CleanSweepLIVE-SelectedWardrobes-Windows.zip)

The download is public. You can play locally without installing Unreal Editor or signing in to TikTok.

## Install on Windows

1. Download the ZIP. In PowerShell, run `Get-FileHash -Algorithm SHA256 "C:\path\to\the\downloaded.zip"` with the path to your ZIP. Continue when the hash matches.
   ```text
   db92109ff3ecf71a03b2436860e4b8ace7a6117c40357fc9b600bc7a291c65c9
   ```
2. Extract the entire ZIP to `%LOCALAPPDATA%\Clean Sweep LIVE`. Keep all the extracted files and folders together, with `CleanSweepLive.exe` directly inside that folder.
3. In File Explorer, right-click `CleanSweepLive.exe` and choose **Send to → Desktop (create shortcut)**. On Windows 11, you may need **Show more options** first. Rename the shortcut **Clean Sweep LIVE**. In shortcut **Properties**, check that **Target** points to the installed EXE and **Start in** points to the install folder. Use the EXE's icon.

The desktop shortcut opens Grungy House. To open Playhouse Park, use `Play Playhouse Park.cmd` in the install folder. See `Controls.txt` for controls.

If Windows reports a missing `VCRUNTIME140` or `MSVCP140` DLL when you launch the game, install the [Microsoft Visual C++ Redistributable (x64)](https://aka.ms/vc14/vc_redist.x64.exe).

## Copy this to a Windows agent

```text
Set up Clean Sweep LIVE for the current user on Windows 10/11 x64.
Download this ZIP:
https://github.com/DSBMediaCreative/UE5-Tests/releases/download/clean-sweep-live-selected-wardrobes-win64/CleanSweepLIVE-SelectedWardrobes-Windows.zip
Verify its SHA-256 before extracting:
db92109ff3ecf71a03b2436860e4b8ace7a6117c40357fc9b600bc7a291c65c9
Extract the whole ZIP to %LOCALAPPDATA%\Clean Sweep LIVE.
Keep all files together with CleanSweepLive.exe at the install root.
Resolve the user's desktop with [Environment]::GetFolderPath('DesktopDirectory')
so the shortcut lands on the actual desktop, including OneDrive redirection.
Create Clean Sweep LIVE.lnk there. Target the full path to CleanSweepLive.exe,
set the working directory to the install folder, and use the EXE's icon.
Check that the EXE exists and that the saved shortcut has the correct target,
working directory, and icon. Report both paths and leave the game closed.
```
