# Fetchly (Beta 0.9.0)
**Universal High-Performance Accessible Media Downloader in Pure Rust**

Developed by **Muhammad Arman** (<arman.munir77@gmail.com>)  
*Proprietary Software. All Rights Reserved.*

---

## Overview

Fetchly is a fast, lightweight, and fully accessible universal media downloader engineered in pure Rust with direct native Win32 Windows API integration. Designed from the ground up for maximum accessibility, it offers a zero-latency experience for visually impaired users navigating via NVDA and JAWS screen readers, as well as an ultra-clean, modern interface for sighted users.

Fetchly supports downloading video and audio from all major media platforms including YouTube (Videos, Shorts, Music, Live), Instagram (Reels, Posts), Facebook (Watch, Reels), TikTok, Twitter/X, SoundCloud, and direct streaming URLs (HLS, DASH, MP4, MP3).

---

## Verified Keyboard Shortcuts Reference

Fetchly features an intuitive, standardized 4-Tab keyboard navigation system with zero mnemonic collisions.

### Global and Navigation Shortcuts

| Shortcut | Action | Scope |
| :--- | :--- | :--- |
| **`Ctrl + Tab`** | Switch to Next Tab (Download -> Settings -> About Us -> Updates) | Global Window |
| **`Ctrl + Shift + Tab`** | Switch to Previous Tab | Global Window |
| **`Alt + P`** | Instantaneous Download Progress Percentage Voice Query | Global Window |
| **`Alt + F4`** | Close Application (Prompts confirmation if download is active) | Global Window |

---

### Tab 1: Download Screen (1 of 4)

| Shortcut | Control / Action | Description |
| :--- | :--- | :--- |
| **`Alt + U`** | Media URL Edit Box | Jump to URL input field |
| **`Alt + L`** | Paste Link Button | Paste URL from clipboard and auto-detect stream |
| **`Alt + V`** | Video (MP4) Radio | Select high-definition video format |
| **`Alt + A`** | Audio Only Radio | Select audio-only format (MP3 / FLAC / AAC) |
| **`Alt + Q`** | Quality Selector | Open quality dropdown (4K, 2K, 1080p, 720p, 320k MP3, etc.) |
| **`Alt + D` / `Enter`**| Start Download | Execute high-speed parallel stream download |
| **`Alt + C` / `Esc`** | Cancel Download | Cancel active download (with safety confirmation) |
| **`Alt + O`** | Play Downloaded Media | Open downloaded file in default Windows media player |
| **`Alt + E`** | Open in Explorer | Reveal and highlight downloaded file in Windows Explorer |
| **`Alt + X`** | Delete File | Remove downloaded file from disk |
| **`Alt + B`** | Back to Main | Return to ready state for a new download |

---

### Tab 2: Settings Screen (2 of 4)

| Shortcut | Control / Action | Description |
| :--- | :--- | :--- |
| **`Alt + F`** | Default Download Folder | Focus download directory path box |
| **`Alt + B`** | Browse Folder Button | Open native Windows folder picker dialog to set new folder |
| **`Alt + M`** | Parallel Multi-Streams | Select concurrency (16 Standard, 32 Turbo, 8 Balanced, 4 Light) |
| **`Alt + T`** | App Theme Selector | Choose theme (System Default, Dark Mode, Light Mode) |
| **`Alt + S`** | Save Preferences | Save folder, quality, parallel streams, and theme settings to disk |

---

### Tab 3: About Us Screen (3 of 4)

| Shortcut | Control / Action | Description |
| :--- | :--- | :--- |
| **`Alt + N`** | Copy Developer Name | Copy "Muhammad Arman" to clipboard |
| **`Alt + M`** | Copy Email Address | Copy "arman.munir77@gmail.com" to clipboard |

---

### Tab 4: Updates Screen (4 of 4)

| Shortcut | Control / Action | Description |
| :--- | :--- | :--- |
| **`Alt + K`** | Check for App Updates | Query GitHub API for new Fetchly releases |
| **`Alt + U`** | Update Core Components | Download and extract latest yt-dlp and FFmpeg binaries |

---

## Key Features

* **Pure Native Win32 GUI:** Built with native Windows controls (`SysTabControl32`, `BUTTON`, `EDIT`), consuming less than 15 MB of RAM with zero Chromium or Electron bloat.
* **Modern Dark and Light Theming Engine:** Windows 11 DWM Immersive Dark title bar, modern charcoal obsidian palette, and instant live theme switching.
* **Direct Screen Reader Integration:** Dynamic bridge to `nvdaControllerClient.dll` and `Tolk.dll` with milestone speech triggers at 25%, 50%, 75%, and 100%.
* **Parallel Multi-Stream Chunk Engine:** Configure 16 (Standard - Default), 32 (Turbo High-Speed), 8 (Balanced), or 4 (Light) concurrent TCP fragments.
* **Accidental Keypress and Exit Protection:** Active downloads cannot be accidentally terminated by `Alt+F4`, `Esc`, or close buttons without explicit confirmation.
* **One-Click Component Auto-Updater:** Integrated background downloader for `yt-dlp.exe`, `ffmpeg.exe`, and `ffprobe.exe` with live progress bars.
* **Pure Rust ID3 and FLAC Metadata Tagger:** Automatically embeds title, artist, track, cover art, and genre tags using the `lofty` engine.

---

## Automated Test Suite

Fetchly includes 58 comprehensive unit and integration tests verifying all core systems:

* `accessibility_tests.rs`: Screen reader voice formatting, milestone math, and shortcut integrity.
* `tab_and_branding_tests.rs`: Tab cycling arithmetic, theme mapping & shortcuts, multi-stream mapping, safety guards, and branding.
* `chunk_and_routing_tests.rs`: Chunk division byte math and platform folder auto-routing.
* `progress_and_regex_tests.rs`: Real-time speed (`MiB/s`, `KiB/s`), ETA, and regex parsers.
* `quality_and_format_tests.rs`: Resolutions (4K to 144p) and audio bitrates (320k to 96kHz FLAC).
* `security_and_sanitizer_tests.rs`: Path traversal stripping, Windows reserved characters, and Urdu Unicode preservation.
* `url_and_extractor_tests.rs`: Platform URL recognition and format resolution.

Run all tests via `run_tests.bat` or:
```cmd
cargo test
```

---

## License and Legal Notice

Proprietary Software.  
Developed by Muhammad Arman. All Rights Reserved.  
Unauthorized distribution, copying, or reverse engineering without explicit written permission from the author is strictly prohibited.
