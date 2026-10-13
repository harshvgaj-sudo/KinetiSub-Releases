# KinetiSub — free tester release

KinetiSub is a Windows and Android caption editor for imported subtitles, animated caption styling, basic video alignment and local MP3 extraction.

This repository hosts downloads and release information. The application source repository is private. The included FFmpeg/LAME corresponding source is available below as required by those libraries' licenses.

## Get the Windows tester build

Open [the latest tester release](https://github.com/harshvgaj-sudo/KinetiSub-Releases/releases) and download the Windows setup EXE. Windows 10/11 x64 and a current Microsoft WebView2 runtime are needed; the installer can obtain WebView2 if it is missing.

**This is a prerelease for testing, not a finished production app.** It is free. No purchase or subscription is offered. The Windows installer is unsigned and may display an unknown-publisher warning. Use the official release assets and compare their SHA-256 checksums; do not disable antivirus or other security protections.

## What it does

- Import SRT, VTT, SBV and timed text; edit captions and review local Hindi-to-Hinglish transliteration.
- Apply 26 curated caption presets, including reference scene compositions and configurable animation.
- Align captions with one video: trim, split, move clips, move captions independently and zoom the timeline up to 30×.
- Export caption videos, subtitle files and locally extracted MP3 audio, using available device encoders.
- Set 3:4 and other custom canvas ratios without cropping the attached footage.

## Important limits

- **Editable sessions are not saved automatically. Export before closing.** SRT/VTT exports do not preserve caption styling or video edits.
- Automatic/local transcription and ad-removal subscription billing are not implemented. Import subtitles created elsewhere.
- This is one-source editing; it does not generate B-roll, separate graphic layers or text behind people.
- Format, resolution and frame-rate support depend on the device encoder. Transparent WebM support also depends on the receiving editor.
- Android store distribution is pending developer-account setup, signing and physical-device checks. Do not mistake an unsigned AAB or a developer debug APK for a production store release.

## Privacy and feedback

Caption/media processing is local; KinetiSub does not upload your files to a KinetiSub server. See [the tester privacy notice](PRIVACY.md).

Report feedback through [this repository's issues](https://github.com/harshvgaj-sudo/KinetiSub-Releases/issues). Include app version, Windows/device version, steps and the observed error. Do not post private videos, credentials or personal information. A short synthetic example is preferable.

## FFmpeg and LAME source and notices

Every binary release must include its exact `KinetiSub-0.1.0-ffmpeg-source.zip`, checksums, third-party notices and LGPL license texts. Download the source archive from the **same release** as the binary. It contains the matching sources, build configuration and replacement instructions. The in-app FFmpeg LGPL notices menu permits loading a compatible modified local core.

KinetiSub uses FFmpeg/LAME for MP3 extraction; caption-video export uses device encoders. Third-party licenses apply to their respective components. Publication of these dependencies' required sources does not license the private application source.
