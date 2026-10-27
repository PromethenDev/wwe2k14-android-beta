# WWE 2K14 Android Beta

An **unofficial fan project**: WWE 2K14 (Xbox 360) running natively on Android phones. This is a **beta** — expect rough edges.

The app does **not** contain the game. You need your own legally obtained copy of WWE 2K14 for Xbox 360.

**Download:** see [Releases](../../releases) — get `WWE2K14-Android-Beta-v0.1.apk` (install directly on the phone) or the `.zip` (APK + guide + notices).

**Help:** [Promethen Projects Discord](https://discord.gg/EFnDwGB332)

## What's in Beta v0.1
- On-screen touch controls (on/off, opacity, size in the launcher). They hide when a controller connects.
- Faster crowd in matches.
- Graphics data is inside the APK, so there are no extra files to copy.
- Performance log + "Send Logs" button in the launcher, so you can help with speed work.

**Updated build (2026-10-27)** - install over your current v0.1, nothing is lost:
- Installing from a disc image (.iso) works from more places: Downloads, SD cards, USB drives and file apps; the .iso
  is no longer greyed out in the file picker.
- Clear messages when something is wrong: a .zip/.7z/.rar instead of an .iso, a damaged or unfinished download, a cloud
  file that is not on the phone yet, or not enough space.
- Retrying after a cancelled install no longer reports "not enough space"; the screen stays on during the install.
- "Send Logs" includes a short install log (no file names). The launcher's left side scrolls; button names are consistent.
- New app icon, the same as the PC version.

## How to install
```
What you need
- Your own WWE 2K14 for Xbox 360 as a disc image (.iso), and the title update 1.0.3 (the update package file, or the
  update already extracted into a folder that has default.xexp in it).
- An Android 12 or newer phone, 64-bit, with Vulkan. It was tested on a Galaxy S23 only.
- Free storage: about 9 GB for the app and the installed game (the game is about 7.8 GB, the app about 0.4 GB).
  If the disc image is on the phone too, it needs its own 7-8 GB while you install; you can delete it afterwards.

Steps
1. Download WWE2K14-Android-Beta-v0.1.apk (about 110 MB) to your phone.
2. Open it. If Android asks, allow your browser or file manager to "install unknown apps", then install.
3. Open "WWE 2K14 Android Beta". The first start unpacks the graphics data (about 280 MB, under a minute on a Galaxy S23).
   Wait until it says "Graphics data is ready". This happens once.
4. Tap "Install from Disc Image" and choose your WWE 2K14 .iso. It can be in Downloads, on an SD card or USB drive,
   or in another file app. Cloud files (Google Drive and similar) must be downloaded to the phone first. The game is
   copied into the app; this takes a few minutes. The screen stays on by itself; keep the phone plugged in.
   If something is wrong (a .zip instead of an .iso, a damaged download, not enough space) the app now says exactly what.
5. Tap "Install Title Update 1.0.3". Choose either "Choose Xbox 360 Update Package File" or "Choose Extracted
   Update Folder" (a folder with default.xexp at its top). It must be installed after the disc image.
6. When the status line says "Game files ready", the game is installed.
7. Optional settings in the launcher (they are remembered):
   - Touch controls: On/Off, Opacity (25-75%), Size (Small/Medium/Large).
   - Picture size: 480p to 4K. 480p or 720p plays best on a phone.
   - Frame rate: Locked 30, 30/60, or 60 Everywhere. "Use Recommended" resets everything.
8. Tap PLAY. On the title screen press Start within about 20 seconds.
9. Controls: with no controller you get on-screen buttons. If you connect a Bluetooth or USB controller they hide
   by themselves and the controller works; turn it off and they come back.
10. Expect about 20-35 fps in matches on a Galaxy S23, and a warm phone. Menus are smooth.

Updating
- Install the new APK over the old one. Do not uninstall first: your saves, game files and settings are kept.

If something is wrong - sending a performance log
1. In the launcher set PERFORMANCE LOG to On (it may cost a tiny bit of speed).
2. Play for a few minutes, close the game, open the launcher and tap "Send Logs".
3. Pick Discord (or any app) in the share sheet. The file holds the game log, your launcher settings, basic phone
   info (model, Android version, GPU, battery temperature) and a short install log (no file names). No game files,
   no personal data.

Help
- Ask in the Promethen Projects Discord: https://discord.gg/EFnDwGB332
- Attach the log file if you have one.
```

## Notices
```
WWE 2K14 (native) for Android - notices

UNOFFICIAL FAN PROJECT. WWE 2K14, its code, characters, names, likenesses and
all game content belong to their rights holders. Not affiliated with WWE, 2K,
Take-Two, Yuke's or Microsoft/Xbox. This app contains NO game files; you must
supply your own legally obtained copy of WWE 2K14 (Xbox 360).

The code written for this project (static recompilation, native renderer,
Android launcher and touch controls) is Copyright the project owner,
ALL RIGHTS RESERVED. It is provided for personal use; it is not licensed for
copying, modification or redistribution. Provided "AS IS", no warranty.

Third-party components included in this app (their licences remain attached):
- ReXGlue SDK / Xenia (BSD-3-Clause) - third-party/third-party-licenses/rexglue-sdk
- plume, Vulkan Memory Allocator, volk, Vulkan-Headers, xxHash - third-party/third-party-licenses/native-renderer
- SDL3 (zlib) - third-party/SDL3-zlib.txt
- libadrenotools (BSD-2-Clause, custom GPU driver loading) - third-party/libadrenotools-BSD-2.txt
- FFmpeg libavcodec / libavutil (LGPL-2.1) - third-party/licenses/FFmpeg-LGPL-2.1.txt and FFmpeg-NOTICE.txt.
  The FFmpeg libraries are separate shared objects (libavcodec.so, libavutil.so) in the app; the matching
  source archive is published with the desktop release (ffmpeg-source-*.zip) and is also provided on request.
- LLVM libc++ (libc++_shared.so, Apache-2.0 with LLVM exception)
```
