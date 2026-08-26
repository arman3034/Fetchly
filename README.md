# Fetchly (Version 0.9.5)
**Universal High-Performance Accessible Media Downloader**

Developed by **Muhammad Arman** (<arman.munir77@gmail.com>)  
*Proprietary Software. All Rights Reserved.*

---

## Welcome to Fetchly

Fetchly is a high-speed, lightweight, and fully accessible media downloader engineered in Native Rust for Windows. Designed from the ground up for zero-lag screen reader accessibility (NVDA, JAWS, Narrator) alongside a clean, modern interface for sighted users.

Fetchly downloads high-fidelity video and audio from all major platforms:
* **YouTube:** Videos, Shorts, Playlists, Channels, YouTube Music, and Live Streams (up to 8K Ultra HD at 60 FPS).
* **Instagram:** Reels, Posts, Stories, and Video Clips.
* **Facebook:** Watch, Reels, and Public Videos.
* **TikTok:** High-Definition Videos with original audio.
* **Twitter / X:** Video Clips and Media attachments.
* **SoundCloud & Bandcamp:** High-quality studio audio streams.
* **Direct URLs:** MP4, MP3, HLS (m3u8), FLV, WebM, and DASH web streams.

---

## Key Features

1. **32-Stream Multi-Chunk Turbo Acceleration:**
   Splits media files into 16 or 32 parallel streams to bypass server speed throttles and maximize your internet bandwidth.

2. **3D Spatial Audio Milestone Chimes (Clash-Free Stereo Panning):**
   Subtle, luxury stereo chimes announce download progress with ear localization: 25% (Left Ear), 50% (Center), 75% (Right Ear), 100% (Grand 3D Stereo Victory Chord) without clashing with NVDA's progress beeps.

3. **Media Inspector & Deep Stream Reader (`Alt + I`):**
   Instantly inspect and hear video titles, accurate durations, available resolutions (8K, 4K, 1080p, MP3), and channel details with a single shortcut.

4. **Speech Verbosity Profiles (Standard / Beginner / Pro Minimalist):**
   Choose your preferred speech experience in Settings: detailed step-by-step guidance for beginners, balanced alerts for standard use, or 90% reduced quiet mode with melodic tones for power users.

5. **Low-Vision Sighted Support & Dynamic Font Zoom:**
   Features a high-contrast Neon Focus Ring for visual clarity and real-time font scaling via `Ctrl + Plus`, `Ctrl + Minus`, and `Ctrl + 0` (from 100% up to 175% Large Print).

6. **Smart Clipboard Auto-Monitor & URL De-Tracking:**
   When you copy any video link, Fetchly automatically strips marketing tracking tags (such as `&si=` and `&fbclid=`) and prepares the clean link instantly with gentle melodic cues and speech alerts.

3. **Platform-Aware Auto-Mode Switching:**
   Copying music links (SoundCloud, YouTube Music) automatically switches Fetchly to Audio Only (MP3 320k) and routes files to your Music folder. Video links automatically configure 1080p Full HD.

4. **Interactive Smart Playlist Checklist:**
   When a playlist is detected, Fetchly displays an interactive checklist with video titles, durations, and range selection. You can download the entire playlist or select individual lessons with the Space bar.

5. **Smart Pause, Resume & Incomplete Task Recovery:**
   If your Wi-Fi disconnects or you pause a download, partial fragments are preserved on disk and can be resumed at any time from the History tab.

6. **Customizable Global Show Hotkey:**
   Press **`Win + Alt + F`** (or your custom chosen letter) from anywhere in Windows to instantly bring Fetchly to the front.

7. **Instant Complete Exit (`Ctrl + Q`):**
   Press **`Ctrl + Q`** inside Fetchly to cleanly terminate the application in 1 millisecond.

8. **Dual Visual Themes:**
   Supports Modern Fluent Charcoal Dark Mode and Clean Studio Light Mode.

---

## User Guide: Quick Start

1. **Copy any media link** in your web browser (e.g. YouTube, TikTok, Facebook).
2. Fetchly will automatically detect the link and announce it. Switch to Fetchly using **`Win + Alt + F`** (or `Alt + Tab`).
3. Choose your format and quality:
   * Press **`Alt + V`** for Video (MP4) or **`Alt + A`** for Audio Only (MP3 / FLAC).
   * Press **`Alt + Q`** to select resolution (8K Ultra HD, 4K, 1080p, 720p, or 320 kbps MP3).
4. Press **`Alt + D`** (or `Enter`) to start downloading.
5. While downloading, press **`Alt + P`** at any time to hear your instant progress percentage and download speed.
6. When download completes, press:
   * **`Alt + O`** to Play the file immediately.
   * **`Alt + E`** to Open the destination folder in Windows Explorer.

---

## Complete Keyboard Shortcuts Reference

Fetchly uses a standardized 5-Tab keyboard layout designed for effortless navigation with zero key collisions.

### Global Shortcuts

| Shortcut | Action |
| :--- | :--- |
| **`Win + Alt + F`** | Show / Restore Fetchly window from anywhere in Windows |
| **`Ctrl + Tab`** | Move to Next Tab |
| **`Ctrl + Shift + Tab`** | Move to Previous Tab |
| **`Alt + P`** | Instantly hear download percentage and speed via Screen Reader |
| **`Ctrl + Plus`** | Zoom In UI Font Size (125%, 150%, 175% Large Print) |
| **`Ctrl + Minus`** | Zoom Out UI Font Size |
| **`Ctrl + 0`** | Reset UI Font Size to 100% Standard |
| **`Ctrl + Q`** | Exit and close Fetchly completely |
| **`Alt + F4`** | Close window (Prompts safety confirmation if download is active) |

---

### Tab 1: Download Screen

| Shortcut | Feature / Action |
| :--- | :--- |
| **`Alt + U`** | Focus Media URL Edit Box |
| **`Alt + L`** | Paste Link from Clipboard manually |
| **`Alt + V`** | Select Video (MP4) Format |
| **`Alt + A`** | Select Audio Only Format |
| **`Alt + Q`** | Open Quality / Resolution Dropdown |
| **`Alt + D` / `Enter`** | Start Download |
| **`Alt + I`** | Inspect Media Metadata (Title, Duration, Qualities, Channel) |
| **`Alt + S`** | Pause Download |
| **`Alt + R`** | Resume Download |
| **`Alt + C` / `Esc`** | Cancel Active Download |
| **`Alt + O`** | Play Downloaded File (Completion View) |
| **`Alt + E`** | Open in Windows Explorer (Completion View) |
| **`Alt + X`** | Delete Downloaded File (Completion View) |

---

### Tab 2: History and Incomplete Screen

| Shortcut | Feature / Action |
| :--- | :--- |
| **`Alt + R`** | Resume Selected Incomplete / Paused Download |
| **`Alt + D`** | Redownload Task from the beginning |
| **`Alt + C`** | Copy Original Media URL to Clipboard |
| **`Alt + O`** | Play Selected Media File |
| **`Alt + E`** | Open Destination Folder in Explorer |
| **`Alt + X`** | Delete Task Record |
| **`Alt + A`** | Clear Entire Download History |

---

### Tab 3: Settings Screen

| Shortcut | Feature / Action |
| :--- | :--- |
| **`Alt + F`** | Focus Default Download Folder Path |
| **`Alt + B`** | Browse and Pick a New Download Folder |
| **`Alt + Q`** | Set Default Video Quality |
| **`Alt + M`** | Set Parallel Streams (16 Standard, 32 Turbo, 8 Balanced, 4 Light) |
| **`Alt + T`** | Set App Theme (System Default, Dark Mode, Light Mode) |
| **`Alt + B`** | Toggle Live Background Clipboard Monitor |
| **`Alt + W`** | Toggle Start Fetchly on Windows Startup |
| **`Alt + K`** | Toggle Global Show Shortcut & Custom Letter Box |
| **`Alt + S`** | Save All Preferences to Disk |

---

### Tab 4: About Us Screen

| Shortcut | Feature / Action |
| :--- | :--- |
| **`Alt + N`** | Copy Developer Name (Muhammad Arman) |
| **`Alt + M`** | Copy Support Email Address (<arman.munir77@gmail.com>) |

---

### Tab 5: Updates Screen

| Shortcut | Feature / Action |
| :--- | :--- |
| **`Alt + K`** | Check for App Updates on GitHub |
| **`Alt + U`** | Download & Update Core Engine Components (yt-dlp, FFmpeg) |
| **`Alt + C`** | Cancel In-Progress Component Update |

---

## Support & Bug Reports

For questions, feature requests, or accessibility feedback:
* **Developer:** Muhammad Arman
* **Email:** <arman.munir77@gmail.com>
