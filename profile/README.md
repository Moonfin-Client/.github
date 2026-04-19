<h1 align="center">Moonfin</h1>
<h3 align="center">Enhanced media streaming clients based on <a href="https://jellyfin.org">Jellyfin</a></h3>

---

<p align="center">
   <img width="1920" height="1080" alt="splash-background" src="https://github.com/user-attachments/assets/c05882da-81ce-47e9-a4b2-c995c337b9b9" />
</p>

## About Moonfin

Moonfin is a collection of enhanced Jellyfin and Emby client applications that build upon the excellent foundation of the official Jellyfin project. We focus on delivering refined user experiences, improved UI/UX, and platform-specific optimizations while maintaining full compatibility with Jellyfin and Emby servers.

Our mission is to provide the best possible viewing experience across all your devices, with thoughtful enhancements that make your media library more accessible and enjoyable to use.

## All Moonfin Clients

Platform | Download | Development Repository
---|---|---
Android Mobile | [Google Play Store](https://play.google.com/store/apps/details?id=org.moonfin.androidtv) | [GitHub/Mobile-Desktop](https://github.com/Moonfin-Client/Mobile-Desktop)
Android TV | [Google Play Store](https://play.google.com/store/apps/details?id=org.moonfin.androidtv) | [GitHub/AndroidTV-FireTV](https://github.com/Moonfin-Client/AndroidTV-FireTV)
iOS | [Apple App Store](https://apps.apple.com/app/moonfin/id6761283970) | [GitHub/Mobile-Desktop](https://github.com/Moonfin-Client/Mobile-Desktop)
Linux | [Latest Github Release](https://github.com/Moonfin-Client/Mobile-Desktop/releases/latest) | [GitHub/Mobile-Desktop](https://github.com/Moonfin-Client/Mobile-Desktop)
MacOS | [Apple App Store](https://apps.apple.com/app/moonfin/id6761283970) | [GitHub/Mobile-Desktop](https://github.com/Moonfin-Client/Mobile-Desktop)
Roku | [Latest Github Release](https://github.com/Moonfin-Client/Roku/releases/latest) | [GitHub/Roku](https://github.com/Moonfin-Client/Roku)
Tizen | [Latest Github Release](https://github.com/Moonfin-Client/Smart-TV/releases/latest) | [GitHub/Smart-TV](https://github.com/Moonfin-Client/Smart-TV)
tvOS | [Apple App Store](https://apps.apple.com/app/moonfin/id6761283970) | [GitHub/tvOS](https://github.com/Moonfin-Client/tvOS)
webOS | [Latest Github Release](https://github.com/Moonfin-Client/Smart-TV/releases/latest) | [GitHub/Smart-TV](https://github.com/Moonfin-Client/Smart-TV)
Windows | [Latest Github Release](https://github.com/Moonfin-Client/Mobile-Desktop/releases/latest) | [GitHub/Mobile-Desktop](https://github.com/Moonfin-Client/Mobile-Desktop)

## What Makes Moonfin Different

Moonfin clients enhance the standard Jellyfin experience with:

- **Modern UI improvements** - Refined layouts, better information density, and smoother animations
- **Enhanced media discovery** - Featured content bars, improved metadata display, and better navigation
- **Emby Support** - All native clients also support Emby Server 4.8.0.0+, so you can connect to Jellyfin or Emby from a single unified app
- **Jellyseerr Integration** - First-class support for content discovery and requesting (first **native** Jellyfin clients with Jellyseerr!)
- **Platform-optimized experiences** - Each client is tailored for its specific device type
- **Server Plugin** - A companion Jellyfin server plugin that brings the Moonfin experience to Jellyfin Web and Mobile, syncs settings across all clients, and proxies Seerr and Jellyseerr
- **Open source** - All improvements are available for the community to use and contribute to

## Core Features (All Clients)

All Moonfin clients share these enhanced features:

- **Cross-Server Content Playback** - First Jellyfin clients with a unified library with seamless playback from multiple Jellyfin and Emby servers in one single UI without having to switch users
- **Profile-aware Featured Media Bar** - Rotating featured content that refreshes per user profile to keep recommendations relevant
- **Emby Support** - All clients support Emby Server 4.8.0.0+ alongside Jellyfin
- **Plugin Sync** - Bidirectional settings sync with the Moonfin Plugin so preferences follow you across devices
- **MDBList Ratings** - Plugin-powered ratings with shared icon/assets support across clients
- **In-player Trailer Previews** - Trailer playback integrated directly into browsing and playback flows
- **Jellyseerr / Seerr Integration** - Browse trending content, request movies/shows in HD/4K/Custom profiles, and track requests
- **Enhanced UI** - Circular cast photos, grouped metadata, taglines, improved contrast and readability
- **Pre-playback Track Selection** - Choose audio/subtitle tracks before playback starts
- **Theme Music Playback** - Background theme music for TV shows and movies with volume control
- **Customizable Navigation** - Shuffle, Genres, and Favorites buttons, plus toolbar visibility, hide/show library rows, and dynamic library button scrolling
- **Subtitle Downloads** - Download subtitles from details screens for online and offline playback
- **Full Playlist Management** - Create playlists, add and remove items, and manage playlist playback across clients
- **Live TV & DVR** - Browse channels, open EPG views, and watch recordings
- **Trickplay** - Thumbnail scrubbing and media segment handling where supported by platform
- **Global Search** - Unified search across Jellyfin libraries and Jellyseerr/Seerr content
- **Cross-Device Settings Sync** - All your preferences sync across every Moonfin client via the server plugin
- **Automatic Updates** - Built-in update checker with in-app notifications

---

## Server Plugin

### [Moonfin Plugin](https://github.com/Moonfin-Client/Plugin)
[![Release](https://img.shields.io/github/release/Moonfin-Client/Plugin.svg)](https://github.com/Moonfin-Client/Plugin/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Plugin/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/Plugin/releases)

**The backbone of the Moonfin ecosystem.** A Jellyfin server plugin used by every client. It acts as the central hub for settings synchronization, Jellyseerr/Seerr integration, and the Moonfin web experience and is what brings Moonfin to Jellyfin Web and the official Mobile app without requiring a separate client.

**Web & Mobile UI Injection**
- Redesigns Jellyfin Web and the Jellyfin Mobile app with the full Moonfin experience, no separate client needed
- Injects a featured media bar, redesigned full-screen details screen, and pill-shaped navigation bar directly into the stock Jellyfin UI
- Embedded Jellyseerr/Seerr panel with automatic SSO via the server proxy
- Home screen row ordering with drag-and-drop reorder and toggle, writes directly to Jellyfin's `DisplayPreferences`
- SyncPlay group watch UI with lobby, group management, and real-time state sync via WebSocket
- All features are optional and toggled per-user from a built-in settings panel; admins can pre-enable defaults for all users

**Cross-Client Settings Sync**
- Per-user preference storage with a per device profile architecture: a shared global base plus sparse overrides for desktop, mobile, and TV, where device profiles only store values that differ from global
- Three-way merge on sync (local wins on conflict); settings follow you when you open Moonfin on a new device
- Admins can set server-wide defaults for any user-facing setting, so new users inherit the full UI out of the box
- Synced settings include: navbar, media bar, details screen, MDBList/TMDB ratings, Jellyseerr rows, home row order, theme music, seasonal effects, parental filters, and more

**Jellyseerr / Seerr Proxy**
- Authenticated reverse proxy that automatically creates browser sessions, so the Jellyseerr iframe loads inside Jellyfin without a separate login
- Supports both Jellyseerr (< 3.0) and Seerr (v3+), and variant is auto-detected
- Clients only need to reach your Jellyfin server; Seerr/Jellyseerr does not need to be directly reachable

**Shared API & Admin Configuration**
- Admin dashboard page in Jellyfin for Seerr URL, display name, enable/disable toggles, and server-wide defaults
- Shared MDBList and TMDB API keys, so individual users do not need their own
- Batch MDBList ratings endpoint, media bar content API, genres API, and TMDB episode ratings proxy used by all native clients
- Serves rating icons as embedded assets (no bundled assets needed in clients)

> **Note:** The plugin is optional for the Jellyfin Web/Mobile experience but **required** for Seerr/Jellyseerr integration in all of the clients and strongly recommended for settings sync across all clients.

**Plugin Setup**

1. In Jellyfin Dashboard → Administration → Plugins → Repositories, add:
   - **Name:** `Moonfin`
   - **URL:** `https://raw.githubusercontent.com/Moonfin-Client/Plugin/refs/heads/master/manifest.json`
2. Go to Catalog → find **Moonfin** → Install
3. Restart Jellyfin
4. For the Web UI, also install the [File Transformation](https://github.com/IAmParadox27/jellyfin-plugin-file-transformation) plugin

---

## Available Clients

### [Android TV / Fire TV](https://github.com/Moonfin-Client/AndroidTV-FireTV/)
[![Release](https://img.shields.io/github/release/Moonfin-Client/AndroidTV-FireTV.svg)](https://github.com/Moonfin-Client/AndroidTV-FireTV/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/AndroidTV-FireTV/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/AndroidTV-FireTV/releases)

**The flagship Moonfin client** for Android TV, Nvidia Shield, and Fire TV devices. Built in Kotlin with Jetpack Compose, derived from the official Jellyfin Android TV client.

**Platform Highlights:**
- **Jetpack Compose UI** - Redesigned libraries, details screens, and dialogs with modern adaptive grids
- **Server Intelligence** - Automatic server type detection, WebSocket real-time events, and feature gating for Jellyfin-only functionality
- **Discovery Enhancements** - Invidious playback with SponsorBlock integration and episode preview overlays on focus
- **Playback Controls** - ASS/SSA subtitles, subtitle delay and positioning, pre-playback track selection, theme music, unpause rewind, and automatic screensaver dimming
- **OTA Updates** - Automatic version checks with in-app installation

**Supported:** Android TV 6.0+, Nvidia Shield, Amazon Fire TV/Stick, Chromecast with Google TV, Google Streamer

---

### [tvOS](https://github.com/Moonfin-Client/tvOS)
[![Release](https://img.shields.io/github/release/Moonfin-Client/tvOS.svg)](https://github.com/Moonfin-Client/tvOS/releases)

**The Moonfin experience on Apple TV**, built natively in Swift and SwiftUI. Designed for the Apple TV remote and the 10-foot viewing experience.

**Platform Highlights:**
- Native SwiftUI interface optimized for Apple TV remote navigation and focus engine
- Top Shelf extension for surfacing continue-watching and featured content on the Apple TV home screen
- Native playback and navigation tuned for the Apple TV 10-foot experience

**Codec Compatibility (from tvOS README):**

| Category | Supported Formats |
|----------|-------------------|
| **Video** | H.264, HEVC (H.265), VP8, VP9, AV1, MPEG-2, MPEG-4, VC-1 |
| **Audio** | AAC, MP3, FLAC, Opus, Vorbis, AC3, EAC3, DTS, TrueHD, PCM, ALAC |
| **Containers** | MP4, MKV, WebM, AVI, MOV, TS / M2TS, WMV / ASF |
| **Subtitles** | SRT, ASS / SSA, VTT / WebVTT, TTML, PGS, DVB, VobSub |
| **HDR** | Dolby Vision, HDR10+, HDR10, HLG |
| **HW Accel** | VideoToolbox on Apple TV hardware |

**Supported:** Apple TV HD and Apple TV 4K (tvOS 16+)

---

### [Mobile & Desktop](https://github.com/Moonfin-Client/Mobile-Desktop)
[![Release](https://img.shields.io/github/release/Moonfin-Client/Mobile-Desktop.svg)](https://github.com/Moonfin-Client/Mobile-Desktop/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Mobile-Desktop/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/Mobile-Desktop/releases)

**A unified Flutter client** for Android, iOS, macOS, Windows, and Linux.

**Platform Highlights:**
- **libmpv via media_kit** - Broad codec coverage across every platform without relying on platform-specific frameworks
- **Downloads** - Original bit-for-bit copy or server-transcoded media (HEVC+AAC up to 50% smaller)
- **Ebooks & Audiobooks** - EPUB, MOBI, AZW, PDF, and comic support, plus M4B and multi-file audiobook playback
- **Integrated Admin Panel** - Server management screens (users, libraries, logs, devices, analytics) built directly into the client
- **Casting and PiP** - Google Cast, DLNA, AirPlay, and picture-in-picture support
- **Custom mpv.conf** - Power-user playback tuning with allowlisted options and optional unsafe advanced mode
- **Desktop** - Full keyboard shortcuts, fullscreen toggle, and SVP frame interpolation support on desktop
- **Parental Controls & PIN** - Content rating restrictions and PIN-protected settings
- **Arch Linux (AUR)** - Available via `yay -S moonfin` or `paru -S moonfin`

**Codec Compatibility (from Mobile-Desktop README):**

| Category | Supported Formats |
|----------|-------------------|
| **Video** | H.264, HEVC (H.265), VP8, VP9, AV1, MPEG-2, MPEG-4, VC-1 |
| **Audio** | AAC, MP3, FLAC, Opus, Vorbis, AC3 (Dolby Digital), EAC3 (Dolby Digital Plus), DTS, TrueHD, PCM (16-/24-bit), ALAC |
| **Containers** | MP4, MKV, WebM, AVI, MOV, TS / M2TS, WMV / ASF |
| **Subtitles** | SRT, ASS / SSA, VTT / WebVTT, TTML, SUB; bitmap (PGS, DVB, VobSub) on desktop |
| **HDR** | Dolby Vision, HDR10+, HDR10, HLG - automatic detection and signaling |
| **HW Accel** | VA-API, QSV, NVENC, VideoToolbox, V4L2, RKMPP |

**Supported:** Android 6.0+, iOS 13+, macOS 10.15+, Windows 10+, Linux (GTK 3)

---

### [Smart TV - Samsung (Tizen) & LG (webOS)](https://github.com/Moonfin-Client/Smart-TV/)
[![Release](https://img.shields.io/github/release/Moonfin-Client/Smart-TV.svg)](https://github.com/Moonfin-Client/Smart-TV/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Smart-TV/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/Smart-TV/releases)

**A unified Smart TV client** built with the React/Enact/Sandstone framework. A single shared codebase powers both Samsung and LG platforms with native video pipelines isolated per platform, AVPlay on Tizen and Starfish/HTML5 on webOS.

**Platform Highlights:**
- **Hardware-accelerated video** - Samsung AVPlay (Tizen) and Starfish/HTML5 (webOS) native pipelines with automatic DirectPlay to native transcode to hls.js fallback
- **UI Polish** - Accent color customization, adjustable blur, UI scale, overlay opacity controls, and smooth featured-banner transitions
- **Automatic screensaver** - Activates after 90 seconds of inactivity to reduce burn-in risk
- Integrates directly with the broader Moonfin ecosystem and settings model

**Supported:** Samsung Smart TVs (Tizen 2.4+, 2016+), LG Smart TVs (webOS 3.0+, 2016+)

---

### [Roku](https://github.com/Moonfin-Client/Roku/)
[![Release](https://img.shields.io/github/release/Moonfin-Client/Roku.svg)](https://github.com/Moonfin-Client/Roku/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Roku/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/Roku/releases)

**An enhanced Roku client** built in BrighterScript and forked from the official Jellyfin Roku client.

**Platform Highlights:**
- **Customizable Navigation** - Pill-shaped sidebar with show/hide controls for key actions and smooth horizontal library scrolling
- **Playback Reliability** - HDR10+ and Dolby Vision fallback handling, subtitle timing offset, and automatic playback retry
- **Updated OSD & Player Styling** - Modernized icon set with improved spacing, layering, and overlay controls
- **Redesigned Details Screen** - Circular cast photos and a unified layout across movies, series, and seasons
- **OTA Updates** - Automatic version checks with in-app notifications
- **Library Customization** - Landscape, portrait, or square grid image orientation

**Supported:** Roku OS 9.1+ (2018+), Roku TV, Streaming Stick, Ultra, Express

---

## Installation & Setup

Each client has its own installation method:

- **Android Mobile / Android TV / Fire TV:** Download from [Google Play Store](https://play.google.com/store/apps/details?id=org.moonfin.androidtv) or grab the APK from releases and sideload (Android 6.0+)
- **tvOS:** Download from the [App Store](https://apps.apple.com/app/moonfin/id6761283970) or sideload via TestFlight
- **iOS / Android Mobile:** Download from the [App Store](https://apps.apple.com/app/moonfin/id6761283970) or [Play Store](https://play.google.com/store/apps/details?id=org.moonfin.androidtv), or sideload from releases
- **macOS / Windows / Linux:** Download installer or binary from [Mobile-Desktop releases](https://github.com/Moonfin-Client/Mobile-Desktop/releases), Linux is also available via AUR (`yay -S moonfin`)
- **Roku:** Download ZIP package from releases and sideload via developer mode (Roku OS 9.1+)
- **Samsung TV (Tizen):** Download WGT from [Smart-TV releases](https://github.com/Moonfin-Client/Smart-TV/releases) and install via [Samsung Jellyfin Installer](https://github.com/PatrickSt1991/Samsung-Jellyfin-Installer) or Tizen Studio (Tizen 2.4+)
- **LG TV (webOS):** Download IPK from [Smart-TV releases](https://github.com/Moonfin-Client/Smart-TV/releases) and install via webOS Dev Manager or `ares-install` (webOS 3.0+)
- **Jellyfin Web & Mobile:** Install the [Moonfin Plugin](https://github.com/Moonfin-Client/Plugin) on your Jellyfin server, no separate client download needed

For detailed installation instructions, visit the specific client or plugin repository.

### Optional: Seerr Setup

To enable media discovery and requesting in Moonfin clients:

1. Install and configure [Seerr](https://seerr.dev/) on your network
2. Configure the Seerr URL in the Moonfin Plugin admin settings (Jellyfin Dashboard → Plugins → Moonfin)
3. The plugin proxies all Seerr requests through your Jellyfin server, so clients only need to reach Jellyfin

## Community & Support

- **Upstream Jellyfin:** [jellyfin.org](https://jellyfin.org)
- **Buy Me a Coffee:** [buymeacoffee.com/moonfin](https://www.buymeacoffee.com/moonfin)
- **Issues & Feature Requests:** Submit in the specific client or plugin repository
- **Discussions:** Available in each repository

## Contributing

We welcome contributions! Moonfin is built on the hard work of the Jellyfin community, and we aim to contribute improvements back upstream where appropriate.

If you're interested in contributing:
1. Check out the specific client or plugin README for build instructions
2. Review open issues and discussions
3. For changes that should go upstream, please coordinate with Jellyfin maintainers
4. Follow the existing code style and conventions for each platform

## Credits

Moonfin builds upon:
- **Jellyfin Project** - The amazing open-source media server and clients
- **MakD's Jellyfin-Media-Bar** - Inspiration for the media bar feature
- **Druidblack** - Original MDBList Ratings plugin
- **Enact/Sandstone** - React-based framework for the Smart TV client
- **MediaLyze** - Inspiration for the admin analytics UI in Mobile & Desktop
- All the contributors to the upstream Jellyfin projects

Special thanks to everyone who has supported Moonfin development through donations and feedback!

## License

Moonfin clients inherit the licenses of their respective upstream projects:
- Android TV / Fire TV: GPL v2
- Mobile & Desktop: GPL v2
- Roku: GPL v2
- Smart TV (Tizen & webOS): MPL 2.0
- Plugin: GPL v3

See individual repositories for specific licensing information.

---

<p align="center">
   <i>Moonfin is not affiliated with the Jellyfin project. It is an independent fork focused on enhanced user experiences.</i>
</p>
