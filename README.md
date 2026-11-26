# Kadrfold

**A simple and fast video editor for Windows, with automatic editing, captions and color.**

> **Early build (beta): v0.1.2.** Kadrfold is free to use during the beta. Expect rough edges and keep backups of important projects and recordings.

**[Download Kadrfold 0.1.2 for Windows](https://github.com/Crimyan/kadrfold/releases/download/v0.1.2-beta/Kadrfold_0.1.2_x64-setup.exe)**

[Polska wersja opisu](README.pl.md)

## What it does

**Editing**

- Timeline with video and audio tracks, trimming, splitting and drag and drop from Explorer.
- Keyframes for position, scale, rotation and opacity.
- Transitions between clips.
- Color correction and adjustment layers that change everything below them.
- Undo and redo for every edit, autosave and recovery after a crash.

**Automatic editing**

- Cuts silence and filler sounds (“um”, “uh”, “yyy”): you see the proposed cuts first and accept them, and one Ctrl+Z brings everything back.
- Lowers music under speech.

**Captions**

- Captions from speech recognition (Whisper) that run on your computer: nothing is sent to the internet.
- Caption translation, also local (Gemma 4 models through llama.cpp, or your own Ollama).
- Caption styles, word-by-word animation, burned into the video or saved as SRT.

**Export**

- MP4 encoded on the graphics card (NVIDIA NVENC; Intel and AMD encoders are used too when available).
- Edit handoff to Premiere Pro (XML) and DaVinci Resolve (FCPXML).

## Install

1. Download **[Kadrfold_0.1.2_x64-setup.exe](https://github.com/Crimyan/kadrfold/releases/download/v0.1.2-beta/Kadrfold_0.1.2_x64-setup.exe)**. All versions: [Releases](../../releases).
2. Run it. It installs for your user only (no administrator rights) into `%LOCALAPPDATA%\Kadrfold` and adds a Start menu shortcut. The installer asks for the language (English or Polski).
3. Windows SmartScreen may warn about an unknown publisher (the beta is not code-signed): choose *More info → Run anyway*.

**Requirements:** Windows 10 or 11 (64-bit), a graphics card with a Vulkan driver (an NVIDIA card is recommended). WebView2 is installed automatically if missing.

To uninstall, use *Settings → Apps* in Windows.

## Models and your data

The installer contains the program and FFmpeg. Speech recognition and translation models are **not** included: Kadrfold downloads them only when you first use captions or translation, and tells you the size before it starts.

Thumbnails, audio waveforms, autosaves and downloaded models are kept in a data folder, by default `%LOCALAPPDATA%\app.kadrfold.desktop`. Models can take several gigabytes, so you can choose another folder or drive in *Help → Data and models folder*. Your recordings and projects stay where you keep them.

## Updates

Kadrfold checks this page for a new version shortly after it starts and every few hours. When there is one, an **↑ Update** button appears in the title bar: install it with one click, after your project is saved. Only the version file is requested from GitHub: nothing about your projects or files is sent. You can turn automatic checking off in *Help → Check for updates*.

## Status

Beta, free, closed source. Found a bug or have an idea? Open an [issue](../../issues): a screenshot and the steps to reproduce help a lot.

## License

Kadrfold is free to download and use during the beta. The source code is not public. See [LICENSE.txt](LICENSE.txt).
© 2026 Crimyan. All rights reserved.

Kadrfold uses third-party components under their own licenses, including FFmpeg under the LGPL (no GPL parts). The full list with license texts is in [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt), in the program folder after installation and in *Help → About and licenses*.
