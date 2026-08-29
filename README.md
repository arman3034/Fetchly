# Fetchly - High-Performance Accessible Media Downloader

**Fetchly** is a native Windows desktop media downloader engineered for ultra-fast parallel multi-stream downloads alongside comprehensive, zero-latency accessibility for blind developers, screen reader navigators (NVDA & Freedom Scientific JAWS), and power users.

---

## Overview

Fetchly allows you to download high-fidelity video and audio from over 1,800+ supported websites (including YouTube, Instagram, Facebook, TikTok, Twitter/X, SoundCloud, Bandcamp, Vimeo, Reddit, Dailymotion, and direct media streams) with clean storage organization, tactile sound feedback, and effortless keyboard navigation.

---

## Key Capabilities

### 1. Parallel Multi-Stream Downloads
* **Multi-Connection Acceleration**: Opens up to 16 or 32 simultaneous connections using Aria2c and yt-dlp to maximize bandwidth.
* **Smart Format Visibility**: Automatically detects audio-only sources (such as SoundCloud, Bandcamp, and YouTube Music), hides video radio buttons, and sets format to MP3/FLAC with screen reader confirmation.
* **Organized Storage Hierarchy**: Neatly categorizes downloaded files inside your `Downloads/Fetchly/` folder (`Fetchly/YouTube`, `Fetchly/Instagram`, `Fetchly/TikTok`, `Fetchly/Facebook`, `Fetchly/Videos`, and `Fetchly/Music`).

### 2. Dual-Engine Screen Reader Accessibility (NVDA & Freedom Scientific JAWS)
* **Zero-Latency Native Speech**: Integrates directly with NVDA Controller Client and Freedom Scientific JAWS (`jfwapi.dll`), with automatic Windows SAPI voice fallback.
* **Milestone Voice Alerts**: Non-intrusive spoken notifications at 25%, 50%, 75%, and 100% download progress.
* **On-Demand Progress Query (`Alt + P`)**: Instantly speaks live percentage, speed, and ETA without disturbing active downloads.

### 3. Visual & Spatial Sensory Explainer (Mental Sight Engine)
* **Focused Control Sight (`Ctrl + Shift + V`)**: Pressing `Ctrl + Shift + V` on any focused button, edit box, radio button, or checkbox plays a precision focal audio cue and speaks its visual styling, pixel dimensions (width/height), screen coordinates, active focus indicator (blinking cursor, dotted marquee, selection dot, checkmark), and exact keyboard interaction rules.
* **Application Visual Overview (`Ctrl + Shift + A`)**: Pressing `Ctrl + Shift + A` plays a panoramic chord and speaks the full visual blueprint of Fetchly—describing the modern download emblem icon, 640x540 window geometry, rounded corners, title bar chrome, 5-tab strip, and central canvas.

### 4. 5-Second Live Audio Stream Probe (`Alt + T`)
* **Hear Before Downloading**: Streams a 5-second audio preview directly to your headphones without saving files to disk, allowing blind users to confirm content before starting large downloads.
* **Instant Stop (`Escape` / `Alt + T`)**: Stop playback immediately at any second.

### 5. High-Definition Embedded Foley Audio Suite
* **Tactile Sound Cues**: High-fidelity sound feedback for modal opening, closing, line navigation, and 3D spatial stereo page flips (`H` sweeps left-to-right, `Shift + H` sweeps right-to-left).
* **Zero External Dependencies**: All sound assets are embedded directly into the binary with pure mathematical DSP generation.

### 6. Accessible Keyboard Shortcuts Reader Modal (`F1` & `Shift + F1`)
* **Context Help (`F1`)**: Opens quick shortcuts for your currently active tab.
* **Master Shortcuts Guide (`Shift + F1`)**: Opens the universal reference guide structured with clear tab headings.
* **Heading Navigation (`H` / `Shift + H`)**: Screen reader users can jump through tab headings with `H` and read line-by-line with Arrow keys.
* **1-Click Actions**: Copy all shortcuts (`Alt + C`), Save guide to Desktop as TXT (`Alt + S`), or Close safely (`Escape`).

### 7. Low-Vision Readability & UI Zoom
* **Dynamic Font Scaling**: Real-time font resizing via `Ctrl + Plus`, `Ctrl + Minus`, and `Ctrl + 0` (from 100% up to 175% Large Print).
* **Dual Theming**: Supports High-Contrast Classic Light Theme and Modern Charcoal Dark Theme.

---

## Universal Keyboard Shortcuts Reference

### Download Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + U` | Focus and select URL input field |
| `Alt + L` | Paste clipboard link into URL field |
| `Alt + V` | Select Video MP4 download mode |
| `Alt + A` | Select Audio MP3 extraction mode |
| `Alt + Q` | Open Quality dropdown to select resolution or bitrate |
| `Alt + D` | Start downloading current media |
| `Alt + C` | Cancel active download safely |
| `Alt + I` | Open Media Inspector to read title, duration, and formats |
| `Alt + T` | Play 5-Second live audio preview probe |
| `Alt + P` | Speak instantaneous download progress percentage |
| `Alt + O` | Play completed downloaded media file |
| `Alt + E` | Open containing directory in Windows Explorer |
| `Alt + X` | Delete completed file from disk |

### Playlist and Queue Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Space` | Toggle focused playlist item checked/unchecked |
| `Alt + S` | Pause currently selected active download in queue |
| `Alt + R` | Resume paused download from partial file |
| `Alt + A` | Select and check all playlist items |
| `Alt + D` | Deselect and uncheck all playlist items |

### Settings Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + B` | Browse and choose custom download folder |
| `Alt + Q` | Select default quality tier |
| `Alt + S` | Configure parallel turbo stream count (16 or 32) |
| `Alt + V` | Select speech verbosity profile (Standard, Beginner, Pro Minimal) |
| `Alt + A` | Save and persist preferences to disk |

### History Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + O` | Play selected media from download history |
| `Alt + E` | Open containing directory in Windows Explorer |
| `Alt + X` | Delete selected file from disk and remove history record |
| `Alt + C` | Clear entire download history list |

### About and Updates Tab
| Shortcut | Action Description |
| :--- | :--- |
| `Alt + N` | Copy developer name (Muhammad Arman) to clipboard |
| `Alt + M` | Copy developer contact email (arman.munir77@gmail.com) |
| `Alt + K` | Check GitHub for new Fetchly application updates |
| `Alt + U` | Check and update core extraction components (yt-dlp, FFmpeg, Deno) |

### Global Application Shortcuts
| Shortcut | Action Description |
| :--- | :--- |
| `Ctrl + Shift + V` | Visual Sight Inspector to hear visual layout and focus indicators of focused control |
| `Ctrl + Shift + A` | Global Application Visual Overview describing icon, window frame, and canvas |
| `F1` | Open quick keyboard shortcuts help for active tab |
| `Shift + F1` | Open Master Keyboard Shortcuts Guide containing all tabs |
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
* **Architecture**: Native x86_64 portable application (no installation or admin rights required)

---

## Developer & Support
* **Lead Architect & Developer**: Muhammad Arman
* **Contact Email**: arman.munir77@gmail.com
* **GitHub Repository**: [arman3034/Fetchly](https://github.com/arman3034/Fetchly)
