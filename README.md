# Fetchly - High-Performance Accessible Media Downloader

**Fetchly** is a native Windows desktop media downloader engineered for ultra-fast parallel multi-stream downloads alongside comprehensive, zero-latency accessibility for blind developers, screen reader navigators (NVDA & Freedom Scientific JAWS), and power users.

---

## Latest Release: v0.9.9 (2026-08-30)
> **What's New**:
> Accessible Playlist Checklist Modal & Multi-Video Downloader, Native Media Player with Master Clock Subtitle Sync, 15 Subtitle Language Tracks, and Smart Context-Aware History Controls.
> * **15 Subtitle Language Tracks**: Dedicated Preferred Subtitle Track dropdown in Settings supporting multi-language embedding and standalone `.SRT` files.
> * **Smart Context-Aware History Controls**: Dynamic button enablement (Resume `Alt+R`, Redownload `Alt+D`, Copy Link `Alt+C`, Play `Alt+P`, Explore `Alt+E`, Delete `Alt+X`, Clear All `Alt+A`).
> * **Adaptive 3-Tier Verbosity Architecture**: Centralized speech and visual inspector formatting for Standard, Beginner, and Pro Minimalist profiles.

---

## Overview

Fetchly allows you to download high-fidelity video and audio from over 1,800+ supported websites (including YouTube, Instagram, Facebook, TikTok, Twitter/X, SoundCloud, Bandcamp, Vimeo, Reddit, Dailymotion, and direct media streams) with clean storage organization, tactile sound feedback, effortless keyboard navigation, and precision segment clipping.

---

## Key Capabilities

### 1. Parallel Multi-Stream Downloads
* **Multi-Connection Acceleration**: Opens up to 16 or 32 simultaneous connections using Aria2c and yt-dlp to maximize bandwidth.
* **Smart Format Visibility**: Automatically detects audio-only sources (such as SoundCloud, Bandcamp, and YouTube Music), hides video radio buttons, and sets format to MP3/FLAC with screen reader confirmation.
* **Organized Storage Hierarchy**: Neatly categorizes downloaded files inside your `Downloads/Fetchly/` folder (`Fetchly/YouTube`, `Fetchly/Instagram`, `Fetchly/TikTok`, `Fetchly/Facebook`, `Fetchly/Videos`, and `Fetchly/Music`).

### 2. Comprehensive Subtitles & Captions Engine
* **15 Subtitle Language Tracks**: Dedicated dropdown in Settings (`English + Urdu`, `Russian`, `Romanian`, `Hindi`, `Arabic`, `Turkish`, `Spanish`, `French`, `German`, `Persian`, `Chinese`, `Japanese`, `Korean`, `English Only`, `All Popular`).
* **Embedded Soft Subtitles (VLC / Media Player Toggle)**: Automatically embeds multi-language subtitles into video containers (MP4/MKV). Sighted and blind users can press `V` in VLC or right-click to toggle subtitles ON/OFF or switch languages.
* **Standalone `.SRT` File Saving**: Saves clean `.srt` subtitle files alongside videos for Refreshable Braille Displays, speech transcripts, and text readers.

### 3. Built-In Accessible Native Player & Lossless Clip Cutter
* **Pure Rust Native Audio Engine**: Direct Windows WaveOut FFI playback with zero third-party player dependencies.
* **Master Hardware Clock Subtitle Sync**: Microsecond-synchronized spoken subtitles and on-screen display without drift.
* **Dialogue Seeking & Spoken Subtitles**: Jump to previous dialogue (`J`), next dialogue (`N`), replay dialogue (`R`), or copy subtitle line to clipboard (`C`).
* **1-Second Lossless Clip Cutter**: Cut instant 30-second (`Ctrl + 3`) or 60-second (`Ctrl + 6`) clips without re-encoding. Set precise In-point (`I`) and Out-point (`O`) and export with `X` / `Ctrl + S`.
* **High-Definition Screenshot Capture**: Press `S` during video playback to save an instant full-resolution PNG frame to Desktop.

### 4. Accessible Time-Trim & Clip Segment Downloader
* **Extract Exact Minutes**: Specify custom Start Time (`Alt + M`) and End Time (`Alt + W`) to download only the desired segment without wasting bandwidth on full multi-hour videos.
* **1-Second Precision Steppers**: Use `-1s` and `+1s` buttons or Up/Down arrows to adjust timestamps in real time with instant speech confirmations.
* **Flexible Time Formats**: Supports both standard time syntax (`HH:MM:SS`, `MM:SS`) and raw seconds (e.g. `90`, `300`).
* **Toggle Segment Mode (`Alt + G`)**: Easily switch between full media download and clipped segment extraction with collision-free ergonomics.

### 5. Dual-Engine Screen Reader Accessibility (NVDA & Freedom Scientific JAWS)
* **Zero-Latency Native Speech**: Integrates directly with NVDA Controller Client and Freedom Scientific JAWS (`jfwapi.dll`), with automatic Windows SAPI voice fallback.
* **Milestone Voice Alerts**: Spoken notifications at 25%, 50%, 75%, and 100% download progress (when enabled).
* **On-Demand Progress Query (`Alt + P`)**: Instantly speaks live percentage, speed, and ETA without disturbing active downloads.

### 6. Visual & Spatial Sensory Explainer (Mental Sight Engine)
* **Focused Control Sight (`Ctrl + Shift + V`)**: Speaks visual styling, colors, WCAG contrast ratio, typography, pixel dimensions (width/height), screen coordinates, surrounding neighbors, and tab order sequence.
* **Application Visual Overview (`Ctrl + Shift + A`)**: Speaks the full visual blueprint of Fetchly—describing the modern download emblem icon, 640x540 window geometry, rounded corners, title bar chrome, 5-tab strip, and central canvas.
* **Adaptive 3-Tier Verbosity**: Automatically formats announcements for Standard, Beginner, and Pro Minimalist profiles.

### 7. 5-Second Live Audio Stream Probe (`Alt + T`)
* **Hear Before Downloading**: Streams a 5-second audio preview directly to your headphones without saving files to disk, allowing blind users to confirm content before starting large downloads.
* **Smart Range Probe**: When Time-Trim mode is active, `Alt + T` automatically plays a 5-second preview starting exactly at your chosen Start Time.
* **Instant Stop (`Escape` / `Alt + T`)**: Stop playback immediately at any second.

### 8. High-Definition Embedded Foley Audio Suite
* **Tactile Sound Cues**: High-fidelity sound feedback for modal opening, closing, line navigation, and 3D spatial stereo page flips (`H` sweeps left-to-right, `Shift + H` sweeps right-to-left).
* **Zero External Dependencies**: All sound assets are embedded directly into the binary with pure mathematical DSP generation.

### 9. Smart Accessible Windows Setup Wizard & Uninstaller
* **Self-Contained Installer (`Fetchly_Setup_v0.9.9.exe`)**: Offline installer bundling all core binaries (`Fetchly.exe`, `yt-dlp.exe`, `ffmpeg.exe`, `aria2c.exe`, `deno.exe`, `Tolk.dll`, and screen reader DLLs).
* **Accessible 4-Page Wizard**: Features full NVDA/JAWS speech announcements and intuitive shortcuts: `&Next` (`Alt + N`), `&Back` (`Alt + B`), `&Install` (`Alt + I`), `&Finish` (`Alt + F`), and `&Cancel` (`Alt + C`).
* **Shortcut Checkboxes**: Customizable `Create &Desktop Shortcut` (`Alt + D`, default unchecked), `Add to &Start Menu` (`Alt + S`, default unchecked), and `Launch Fetchly Now` (`Alt + L`, default checked).
* **Active Process Detection**: Automatically detects running instances of Fetchly and prompts to cleanly close and overwrite without corrupting files.
* **Clean Uninstaller (`uninstall.exe`)**: Registered in Windows Programs and Features (Installed Apps) under publisher "Muhammad Arman", with options to keep or purge download history.
* **Silent Auto-Update Mode (`/SILENT`)**: Supports background 1-click upgrades when triggered from Fetchly's Updates Tab.

### 10. Low-Vision Readability & UI Zoom
* **Dynamic Font Scaling**: Real-time font resizing via `Ctrl + Plus`, `Ctrl + Minus`, and `Ctrl + 0` (from 100% up to 175% Large Print).
* **Dual Theming**: Supports High-Contrast Classic Light Theme and Modern Charcoal Dark Theme.

---

## Universal Keyboard Shortcuts Reference

### 1. Download Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + U` | Focus and select URL input field |
| `Alt + L` | Paste clipboard link into URL field |
| `Alt + V` | Select Video MP4 download mode |
| `Alt + A` | Select Audio MP3 extraction mode |
| `Alt + Q` | Open Quality dropdown to select resolution or bitrate |
| `Alt + G` | Toggle Time-Trim / Segment Clip download mode |
| `Alt + M` | Focus Start Time (From) box |
| `Alt + W` | Focus End Time (To) box |
| `Alt + D` | Start downloading current media |
| `Alt + C` | Cancel active download safely |
| `Alt + I` | Open Media Inspector to read title, duration, and formats |
| `Alt + T` | Play 5-Second live audio preview probe (trimmed range when active) |
| `Alt + P` | Speak instantaneous download progress percentage |
| `Alt + O` | Play completed downloaded media file |
| `Alt + E` | Open containing directory in Windows Explorer |
| `Alt + X` | Delete completed file from disk |

### 2. History and Incomplete Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + R` | Resume selected paused or incomplete download task |
| `Alt + D` | Redownload selected item from source link |
| `Alt + C` | Copy media source link to clipboard |
| `Alt + P` | Play selected completed media in built-in player |
| `Alt + E` | Open containing directory in Windows Explorer |
| `Alt + X` | Delete selected file from disk and remove history record |
| `Alt + A` | Clear entire download history list |

### 3. Settings Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + B` | Browse and choose custom download folder |
| `Alt + Q` | Select default quality tier |
| `Alt + M` | Configure parallel turbo stream count (16 or 32) |
| `Alt + T` | Select application visual theme (Auto / Dark / Light) |
| `Alt + V` | Select speech verbosity profile (Standard, Beginner, Pro Minimal) |
| `Alt + C` | Toggle audio chimes sound feedback |
| `Alt + E` | Toggle soft subtitles embedding for video |
| `Alt + S` | Save and persist preferences to disk |
| `Alt + W` | Toggle start Fetchly on Windows startup |
| `Alt + U` | Toggle check for updates automatically on startup |
| `Alt + H` | Enable global show hotkey (Win+Alt+F) |

### 4. About Us Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + N` | Copy developer name (Muhammad Arman) to clipboard |
| `Alt + M` | Copy developer contact email (arman.munir77@gmail.com) |

### 5. Updates Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + K` | Check GitHub for new Fetchly application updates |
| `Alt + U` | Check and update core extraction components (yt-dlp, FFmpeg, Deno) |

### 6. Built-In Accessible Native Player Shortcuts
| Shortcut | Action Description |
| :--- | :--- |
| `Spacebar` / `K` | Play or Pause media playback |
| `Left` / `Right Arrow` | Seek 5 seconds backward or forward |
| `Shift + Left / Right` | Seek 30 seconds backward or forward |
| `Ctrl + Left / Right` | Seek 1 minute backward or forward |
| `0` to `9` | Jump directly to percentage of media (1 = 10%, 5 = 50%, 0 = Start) |
| `Home` / `End` | Jump to beginning (00:00) or near end |
| `Up` / `Down Arrow` | Increase or decrease volume by 5% |
| `M` | Mute or unmute audio |
| `]` / `[` | Increase or decrease playback speed (0.5x to 3.0x) |
| `Backspace` | Reset playback speed to normal 1.0x |
| `T` / `Alt + P` | Speak exact elapsed, remaining time and percentage |
| `L` | Cycle subtitle language tracks (Urdu, English, Arabic, Romanian, etc.) |
| `V` | Toggle Spoken Subtitles voice output on/off |
| `J` / `N` | Jump to previous or next subtitle sentence dialogue |
| `R` | Replay current subtitle sentence dialogue from start |
| `C` | Copy active subtitle line to clipboard |
| `I` / `[` | Set Lossless Clip Start In-Point |
| `O` / `]` | Set Lossless Clip End Out-Point |
| `X` / `Ctrl + S` | Export Lossless Cut Clip in 1 second |
| `Ctrl + 3` | Quick Cut 30-Second Clip from current position |
| `Ctrl + 6` | Quick Cut 60-Second (1 Minute) Clip from current position |
| `S` | Capture High-Definition PNG Screenshot frame to Desktop |
| `F` / `Alt + Enter` | Toggle full-screen video canvas |
| `Alt + E` | Reveal media file in Windows Explorer |
| `Escape` | Close native player and return to Fetchly |

### 7. Global Application Shortcuts
| Shortcut | Action Description |
| :--- | :--- |
| `Ctrl + Shift + V` | Visual Sight Inspector to hear visual layout and focus indicators of focused control |
| `Ctrl + Shift + A` | Global Application Visual Overview describing icon, window frame, and canvas |
| `F1` | Open quick keyboard shortcuts help for active tab |
| `Shift + F1` | Open Master Keyboard Shortcuts Guide containing all 5 tabs |
| `Ctrl + Tab` | Switch forward to next tab |
| `Ctrl + Shift + Tab` | Switch backward to previous tab |
| `Ctrl + Plus` | Increase user interface font size (125%, 150%, 175%) |
| `Ctrl + Minus` | Decrease user interface font size |
| `Ctrl + 0` | Reset font size back to default 100% |
| `Win + Alt + F` | Global hotkey to bring Fetchly window to foreground |
| `Ctrl + Q` | Cleanly exit Fetchly |
| `Escape` | Close active dialog / stop audio probe / restore focus |

---

## System Requirements
* **Operating System**: Windows 10 or Windows 11 (64-bit recommended)
* **Screen Reader Support**: NVDA, Freedom Scientific JAWS, or Windows SAPI
* **Architecture**: Available as standalone setup installer (`Fetchly_Setup_v0.9.9.exe`) or portable zip (`Fetchly_v0.9.9_Portable.zip`)

---

## Developer & Support
* **Lead Architect & Developer**: Muhammad Arman
* **Contact Email**: arman.munir77@gmail.com
* **GitHub Repository**: [arman3034/Fetchly](https://github.com/arman3034/Fetchly)
