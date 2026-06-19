<h1 align="center">Moonfin</h1>
<h3 align="center">Premium media streaming clients for Jellyfin and Emby</a></h3>

---

<p align="center">
   <img width="1920" height="1080" alt="splash-background" src="https://github.com/user-attachments/assets/c05882da-81ce-47e9-a4b2-c995c337b9b9" />
</p>

## About Moonfin

Moonfin is a collection of premium Jellyfin and Emby client applications. We focus on delivering refined user experiences, improved UI/UX, and platform-specific optimizations while maintaining full compatibility with Jellyfin and Emby servers.

Our mission is to provide the best possible viewing experience across all your devices, with thoughtful enhancements that make your media library more accessible and enjoyable to use.

## All Moonfin Clients

Platform | Download | Development Repository
---|---|---
Android Mobile | [![Google Play](https://img.shields.io/badge/Google%20Play-grey?logo=Google+Play\&label=)](https://play.google.com/store/apps/details?id=org.moonfin.androidtv) | [GitHub/Moonfin-Core](https://github.com/Moonfin-Client/Moonfin-Core)
Android TV | [![Google Play](https://img.shields.io/badge/Google%20Play-grey?logo=Google+Play\&label=)](https://play.google.com/store/apps/details?id=org.moonfin.androidtv) | [GitHub/Moonfin-Core](https://github.com/Moonfin-Client/Moonfin-Core)
iOS | [![App Store](https://img.shields.io/badge/App%20Store-grey?logo=apple&label=)](https://apps.apple.com/app/moonfin/id6761283970) | [GitHub/Moonfin-Core](https://github.com/Moonfin-Client/Moonfin-Core)
Linux | [Latest Github Release](https://github.com/Moonfin-Client/Moonfin-Core/releases/latest) | [GitHub/Moonfin-Core](https://github.com/Moonfin-Client/Moonfin-Core)
MacOS | [![App Store](https://img.shields.io/badge/App%20Store-grey?logo=apple&label=)](https://apps.apple.com/app/moonfin/id6761283970) | [GitHub/Moonfin-Core](https://github.com/Moonfin-Client/Moonfin-Core)
Roku | [![Roku](https://img.shields.io/badge/Roku-grey?logo=Roku&label=)](https://channelstore.roku.com/details/92a83c9f4112b76a7bcee3dc076254ca:3251a91bf7af7339652d5409ccfdcb39/moonfin)  | [GitHub/Roku](https://github.com/Moonfin-Client/Roku)
Tizen | [Latest Github Release](https://github.com/Moonfin-Client/Smart-TV/releases/latest) | [GitHub/Smart-TV](https://github.com/Moonfin-Client/Smart-TV)
tvOS | [![App Store](https://img.shields.io/badge/App%20Store-grey?logo=apple&label=)](https://apps.apple.com/app/moonfin/id6761283970) | [GitHub/Moonfin-Core](https://github.com/Moonfin-Client/Moonfin-Core)
webOS | [Latest Github Release](https://github.com/Moonfin-Client/Smart-TV/releases/latest) | [GitHub/Smart-TV](https://github.com/Moonfin-Client/Smart-TV)
Windows | [Latest Github Release](https://github.com/Moonfin-Client/Moonfin-Core/releases/latest) | [GitHub/Moonfin-Core](https://github.com/Moonfin-Client/Moonfin-Core)

## What Makes Moonfin Different

Moonfin clients enhance the standard Jellyfin experience with:

- **Modern UI improvements** - Refined layouts, better information density, and smoother animations
- **Enhanced media discovery** - Featured content bars, improved metadata display, and better navigation
- **Emby Support** - All native clients also support Emby Server 4.8.0.0+, so you can connect to Jellyfin or Emby from a single unified app
- **Seerr Integration** - First-class support for content discovery and requesting (first **native** Jellyfin clients with Seerr!)
- **Platform-optimized experiences** - Each client is tailored for its specific device type
- **Server Plugin** - A companion Jellyfin server plugin that brings the Moonfin experience to Jellyfin Web and Mobile, syncs settings across all clients, and proxies Seerr, MDBList, and TMDB
- **Open source** - All improvements are available for the community to use and contribute to

## Core Features (All Clients)

All Moonfin clients share these enhanced features:

- **Cross-Server Content Playback** - First Jellyfin clients with a unified library with seamless playback from multiple Jellyfin and Emby servers in one single UI without having to switch users
- **Profile-aware Featured Media Bar** - Rotating featured content that refreshes per user profile to keep recommendations relevant
- **Emby Support** - All clients support Emby Server 4.8.0.0+ alongside Jellyfin
- **Plugin Sync** - Bidirectional settings sync with the Moonfin Plugin so preferences follow you across devices
- **MDBList Ratings** - Plugin-powered ratings with shared icon/assets support across clients
- **In-player Trailer Previews** - Trailer playback integrated directly into browsing and playback flows
- **Seerr Integration** - Browse trending content, request movies/shows in HD/4K/Custom profiles, and track requests
- **Enhanced UI** - Circular cast photos, grouped metadata, taglines, improved contrast and readability
- **Pre-playback Track Selection** - Choose audio/subtitle tracks before playback starts
- **Theme Music Playback** - Background theme music for TV shows and movies with volume control
- **Customizable Navigation** - Shuffle, Genres, and Favorites buttons, plus toolbar visibility, hide/show library rows, and dynamic library button scrolling
- **Subtitle Downloads** - Download subtitles from details screens for online and offline playback
- **Full Playlist Management** - Create playlists, add and remove items, and manage playlist playback across clients
- **Live TV & DVR** - Browse channels, open EPG views, and watch recordings
- **Trickplay** - Thumbnail scrubbing and media segment handling where supported by platform
- **Global Search** - Unified search across Jellyfin libraries and Seerr content
- **Cross-Device Settings Sync** - All your preferences sync across every Moonfin client via the server plugin
- **Automatic Updates** - Built-in update checker with in-app notifications

---

## Server Plugin

### [Moonbase Plugin](https://github.com/Moonfin-Client/Plugin)

[![Release](https://img.shields.io/github/release/Moonfin-Client/Plugin.svg)](https://github.com/Moonfin-Client/Plugin/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Plugin/total?logo=github\&label=Downloads)](https://github.com/Moonfin-Client/Plugin/releases)

**The backbone of the Moonfin ecosystem.** Moonbase is a multi-purpose Jellyfin server plugin that provides the shared infrastructure used by Moonfin clients. It handles settings synchronization, runtime web configuration and discovery, server-side API proxying, Seerr integration, admin configuration, custom themes, and the hosted Moonfin web experience.

Moonbase also serves the Moonfin web interface directly from Jellyfin at `/Moonfin/Web/`, allowing the Moonfin web app to run side-by-side with Jellyfin Web. With the optional File Transformation bridge, admins can add a Moonfin icon to the stock Jellyfin Web header for one-click access.

**Moonfin Web Hosting**

* Serves the full Moonfin web app directly from Jellyfin at `/Moonfin/Web/`
* Provides runtime web configuration and discovery endpoints for same-origin plugin mode startup
* Serves embedded Moonfin web assets and rating icons from the plugin
* Includes a diagnostics route for troubleshooting web startup and routing issues

**Cross-Client Settings Sync**

* Stores per-user Moonfin preferences on the server
* Supports a shared global profile plus optional desktop, mobile, and TV profile overrides
* Device profiles only store values that differ from global, so global changes automatically flow to devices unless explicitly overridden
* Supports bidirectional sync with local-wins conflict behavior
* Provides optional real-time settings and theme refresh events through `/Moonfin/Settings/Stream`
* Lets admins define server-wide defaults for user-facing settings
* Lets admins push current defaults to already-initialized user profiles

**Seerr Proxy & SSO**

* Provides an authenticated Seerr API proxy routed through Jellyfin
* Handles Seerr session access for Moonfin clients
* Lets clients use Seerr features without requiring Seerr to be directly reachable by every device
* Requires reverse proxies to forward `/Moonfin/` paths to Jellyfin, including Seerr API traffic through `/Moonfin/Jellyseerr/Api/`

**Shared Server APIs**

* Provides shared MDBList and TMDB proxy endpoints so API keys stay server-side
* Provides media bar, genre, ratings, and metadata helper APIs used by Moonfin clients
* Hosts shared rating icons and embedded assets
* Provides admin broadcast messages for sending announcements to connected users

**Admin Configuration**

* Adds a Moonfin plugin page under Jellyfin Dashboard → Plugins → Moonfin
* Lets admins configure Seerr URL, display name, enable/disable toggles, shared API keys, server defaults, settings sync, and web runtime options
* Supports custom theme upload, validation, and metadata tracking
* Includes a built-in theme editor at `/Moonfin/Web/theme/`

> **Note:** Moonbase is strongly recommended for all Moonfin users. It is required for Seerr integration and provides the best experience for settings sync, shared server-side APIs, custom themes, and the hosted Moonfin web app.

**Plugin Setup**

1. In Jellyfin Dashboard → Administration → Plugins → Repositories, add:

   * **Name:** `Moonfin`
   * **URL:** `https://raw.githubusercontent.com/Moonfin-Client/Plugin/refs/heads/master/manifest.json`
2. Go to Catalog → find **Moonfin** → Install
3. Restart Jellyfin
4. Open the Moonfin web app at:

   * `https://your-jellyfin-host/Moonfin/Web/`
5. If assets do not appear after a fresh install, run the **Moonfin Startup** task from Jellyfin Dashboard → Administration → Scheduled Tasks, then refresh the page

**Optional Jellyfin Web Header Link**

To add a Moonfin icon to the stock Jellyfin Web header:

1. Add the File Transformation plugin repository to Jellyfin:

   * **URL:** `https://www.iamparadox.dev/jellyfin/plugins/manifest.json`
2. Install the **File Transformation** plugin from the catalog
3. Restart Jellyfin
4. Force refresh your browser
5. Click the Moonfin icon next to SyncPlay

---

### [Android TV / Fire TV](https://github.com/Moonfin-Client/Moonfin-Core/)

[![Release](https://img.shields.io/github/release/Moonfin-Client/Moonfin-Core.svg)](https://github.com/Moonfin-Client/Moonfin-Core/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Moonfin-Core/total?logo=github\&label=Downloads)](https://github.com/Moonfin-Client/Moonfin-Core/releases) [![Google Play](https://img.shields.io/badge/Google%20Play-grey?logo=Google+Play&label=)](https://play.google.com/store/apps/details?id=org.moonfin.androidtv)

**The flagship Moonfin client** for Android TV, Nvidia Shield, Fire TV, Chromecast with Google TV, Google Streamer, and other Android-based TV devices. Built from the shared Moonfin Core codebase and adapted for remote-first living-room use, it brings the Moonfin experience to TV screens with Jellyfin and Emby support, TV-focused playback, and deep integration with the Moonfin plugin ecosystem.

**Platform Highlights:**

* **TV-Optimized Interface** - A living-room-focused Moonfin experience adapted for remote navigation, large-screen browsing, couch-friendly layouts, and Android-based TV devices
* **Media3 / ExoPlayer Playback** - Uses Android's Media3 / ExoPlayer playback stack for TV-focused video playback, subtitles, track selection, audio passthrough, and hardware-backed playback behavior
* **Remote-First Navigation** - Sidebar navigation, focus-friendly layouts, dynamic library shortcuts, folder browsing, shuffle controls, and configurable toolbar behavior
* **TV Playback Controls** - ASS/SSA subtitle support, subtitle delay and positioning, pre-playback audio/subtitle selection, max video resolution preference, unpause rewind, next episode countdown, trickplay scrubbing, and automatic screensaver dimming
* **Living-Room Discovery** - Featured media, rich item details, trailers, theme music, ratings, genres, and Seerr request flows presented in a TV-friendly interface
* **Plugin Integration** - Uses the Moonfin server plugin for synced preferences, shared ratings, Seerr proxy access, media bar data, rating icons, and server-side configuration
* **OTA Updates** - Built-in version checks with in-app update notifications and update availability prompts

**Supported:** Android TV 6.0+, Nvidia Shield, Amazon Fire TV/Stick, Chromecast with Google TV, Google Streamer

---

### [Apple TV (tvOS)](https://github.com/Moonfin-Client/Moonfin-Core)

[![Release](https://img.shields.io/github/release/Moonfin-Client/Moonfin-Core.svg)](https://github.com/Moonfin-Client/Moonfin-Core/releases) [![App Store](https://img.shields.io/badge/App%20Store-grey?logo=apple&label=)](https://apps.apple.com/app/moonfin/id6761283970)

**The Moonfin experience on Apple TV**, now built from the shared Moonfin Core codebase (Flutter via the flutter-tvos toolchain) with a native MPVKit playback core. Previously a standalone app, the Apple TV client now shares the same home screen, themes, and settings as every other Moonfin platform while keeping a native, hardware-accelerated player tuned for the Siri Remote and the 10-foot living-room experience.

**Platform Highlights:**

* **Shared Flutter Interface** - The same Moonfin home screen, browsing, and settings as mobile, desktop, and Android TV, tuned for the Apple TV focus engine and Siri Remote navigation
* **Native MPVKit Playback** - Hardware-accelerated playback with Dolby Vision Profile 7 decode and Atmos passthrough, advertised only when the connected display actually supports it
* **Living-Room Player** - Full native player OSD with trickplay, track pickers, a quality menu, cast and crew, skip intro and credits, a Still Watching prompt, and SyncPlay controls
* **System Integration** - Top Shelf and app icon, Now Playing with remote commands, theme music, AirPlay, and a TV screensaver with idle tracking
* **Live TV** - Live TV browsing and playback tuned for Apple TV

**Codec Compatibility:**

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

### [Moonfin Core](https://github.com/Moonfin-Client/Moonfin-Core)

[![Release](https://img.shields.io/github/release/Moonfin-Client/Moonfin-Core.svg)](https://github.com/Moonfin-Client/Moonfin-Core/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Moonfin-Core/total?logo=github\&label=Downloads)](https://github.com/Moonfin-Client/Moonfin-Core/releases) [![Google Play](https://img.shields.io/badge/Google%20Play-grey?logo=Google+Play\&label=)](https://play.google.com/store/apps/details?id=org.moonfin.androidtv) [![App Store](https://img.shields.io/badge/App%20Store-grey?logo=apple&label=)](https://apps.apple.com/app/moonfin/id6761283970)

**A unified Flutter client** for mobile, tablet, desktop, web, and experimental Samsung TV builds, and the shared codebase that also powers the Moonfin Android TV and Apple TV apps. Moonfin Core is designed for Jellyfin and Emby users who want a modern, customizable media experience across Android, iOS, macOS, Windows (x64 and ARM64), Linux, web, and Tizen.

**Platform Highlights:**

* **Cross-Platform Flutter App** - One shared Flutter codebase optimized for **phones, tablets, desktop environments, and web**, and shared with the Android TV and Apple TV clients plus experimental Tizen / Samsung TV builds
* **Jellyfin & Emby Support** - Supports Jellyfin 10.8.0+ and Emby 4.8.0.0+ with unified browsing, playback, search, and library management
* **Per-Platform Playback Backends** - Mobile, desktop, and web use `media_kit` / libmpv for broad codec, subtitle, HDR, and hardware acceleration support, while the Android TV and Apple TV clients use native Media3/ExoPlayer and MPVKit backends respectively
* **Web (PWA)** - Builds as an installable progressive web app served by the Moonbase server plugin, with an in-browser theme editor
* **Tizen Playback Path** - Experimental Samsung TV builds use Tizen AVPlay through the Tizen video player stack instead of libmpv / ExoPlayer, with platform-specific limitations
* **Downloads** - Download media as an original bit-for-bit copy or as a smaller server-transcoded file using HEVC video, AAC audio, and MP4 container presets
* **Offline Playback** - Downloaded media is automatically organized by media type, with resume tracking, offline subtitles, and full playback controls for downloaded content
* **Ebooks & Audiobooks** - Read EPUB, MOBI, AZW/AZW3, PDF, and comic archives, plus play M4B and multi-file audiobooks with chapters, bookmarks, resume support, and offline downloads
* **Multi-Server Unified Library** - Connect to multiple Jellyfin and/or Emby servers at the same time and browse, search, continue, and play content from one unified interface
* **Integrated Admin Panel** - Manage server settings, users, libraries, logs, devices, and analytics directly from the client
* **Casting & Session Control** - Includes Google Cast, DLNA, and AirPlay integration paths, plus remote playback/session controls, track selection, delay controls, queue behavior, and picture-in-picture support
* **Advanced Playback Controls** - Subtitle and audio delay adjustment, pre-playback track selection, ongoing track control, still-watching flow, next-up handling, trickplay previews, and media segment handling
* **Featured Media & Home Customization** - Rotating hero content, multiple media bar layouts, rich backdrop presentation, configurable home rows, a Theme Store, and plugin-compatible home row preference sync
* **Ratings & Metadata** - Optional MDBList and TMDB ratings, TMDB episode ratings, customizable rating display, rich item details, trailers, and enhanced metadata presentation
* **Live TV & DVR** - Live TV browsing and playback, EPG-style guide views, DVR recordings, and schedule management screens
* **Parental Controls & PIN** - PIN-protected sensitive actions/settings and configurable content rating restrictions
* **Automatic Updates** - Built-in update checks with configurable cadence and in-app update availability prompts
* **Desktop Builds** - Windows installer (x64 and native ARM64), macOS DMG, macOS app bundle, and Linux package outputs including tarball, AppImage, deb, rpm, snap, and flatpak depending on available tooling
* **Tizen Builds** - Experimental Samsung TV `.tpk` builds through `flutter-tizen`, Tizen Studio, and a signed Tizen security profile

**Codec Compatibility (from Moonfin-Core README):**

| Category       | Supported Formats                                                                                                 |
| -------------- | ----------------------------------------------------------------------------------------------------------------- |
| **Video**      | H.264, HEVC (H.265), VP8, VP9, AV1, MPEG-2, MPEG-4, VC-1                                                          |
| **Audio**      | AAC, MP3, FLAC, Opus, Vorbis, AC3 (Dolby Digital), EAC3 (Dolby Digital Plus), DTS, TrueHD, PCM (16-/24-bit), ALAC |
| **Containers** | MP4, MKV, WebM, AVI, MOV, TS / M2TS, WMV / ASF                                                                    |
| **Subtitles**  | SRT, ASS / SSA, VTT / WebVTT, TTML, SUB; bitmap subtitles such as PGS, DVB, and VobSub on desktop                 |
| **HDR**        | Dolby Vision, HDR10+, HDR10, HLG, with automatic detection and signaling                                          |
| **HW Accel**   | VA-API, QSV, NVENC, VideoToolbox, V4L2, RKMPP                                                                     |

**Supported:** Android 6.0+ / API 23+, iOS 13.0+, macOS 10.15+, Windows 10+ (x64 and ARM64), Linux with GTK 3 and CMake 3.13+, web (installable PWA), Tizen 6.0+ experimental

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
[![Release](https://img.shields.io/github/release/Moonfin-Client/Roku.svg)](https://github.com/Moonfin-Client/Roku/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Roku/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/Roku/releases) [![Roku](https://img.shields.io/badge/Roku-grey?logo=Roku&label=)](https://channelstore.roku.com/details/92a83c9f4112b76a7bcee3dc076254ca:3251a91bf7af7339652d5409ccfdcb39/moonfin) 

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
- **macOS / Windows / Linux:** Download installer or binary from [Moonfin-Core releases](https://github.com/Moonfin-Client/Moonfin-Core/releases), Windows ships both x64 and native ARM64 installers, and Linux is also available via AUR (`yay -S moonfin`)
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
- Mobile, Desktop & Apple TV: GPL v2
- Roku: GPL v2
- Smart TV (Tizen & webOS): MPL 2.0
- Plugin: GPL v3

See individual repositories for specific licensing information.

---

<p align="center">
   <i>Moonfin is not affiliated with the Jellyfin project. It is an independent fork focused on enhanced user experiences.</i>
</p>
