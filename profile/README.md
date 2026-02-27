<h1 align="center">Moonfin</h1>
<h3 align="center">Enhanced media streaming clients based on <a href="https://jellyfin.org">Jellyfin</a></h3>

---

<p align="center">
   <img width="4305" height="2659" alt="splash-background" src="https://github.com/user-attachments/assets/8618363e-d982-4828-8274-a2c3c7623ddb" />
</p>

## About Moonfin

Moonfin is a collection of enhanced Jellyfin client applications that build upon the excellent foundation of the official Jellyfin project. We focus on delivering refined user experiences, improved UI/UX, and platform-specific optimizations while maintaining full compatibility with Jellyfin servers.

Our mission is to provide the best possible viewing experience across all your devices, with thoughtful enhancements that make your media library more accessible and enjoyable to use.

## What Makes Moonfin Different

Moonfin clients enhance the standard Jellyfin experience with:

- **Modern UI improvements** - Refined layouts, better information density, and smoother animations
- **Enhanced media discovery** - Featured content bars, improved metadata display, and better navigation
- **Jellyseerr Integration** - First-class support for content discovery and requesting (first **native** Jellyfin clients with Jellyseerr!)
- **Platform-optimized experiences** - Each client is tailored for its specific device type
- **Server Plugin** - A companion Jellyfin server plugin that brings the Moonfin experience to Jellyfin Web and Mobile, syncs settings across all clients, and proxies Seerr andJellyseerr
- **Open source** - All improvements are available for the community to use and contribute to

## Core Features (All Clients)

All Moonfin clients share these enhanced features:

-  **Cross-Server Content Playback** - First Jellyfin clients with a unified library with seamless playback from multiple Jellyfin servers in one single UI without having to switch users
-  **Jellyseerr Integration** - Browse trending content, request movies/shows in HD/4K/Custom profiles, and track requests
-  **Enhanced UI** - Circular cast photos, grouped metadata, taglines, improved contrast and readability
-  **Pre-playback Track Selection** - Choose audio/subtitle tracks before playback starts
-  **Theme Music Playback** - Background theme music for TV shows and movies with volume control
-  **Customizable Navigation** - Shuffle, Genres, and Favorites buttons. Toggle toolbar visibility, hide/show library rows, dynamic library buttons with scrolling
-  **Global Search** - Unified search across Jellyfin libraries and Jellyseerr content
-  **Cross-Device Settings Sync** - All your preferences sync across every Moonfin client via the server plugin
-  **Automatic Updates** - Built-in update checker with in-app notifications

## Server Plugin

### [Moonfin Plugin](https://github.com/Moonfin-Client/Plugin)
[![Release](https://img.shields.io/github/release/Moonfin-Client/Plugin.svg)](https://github.com/Moonfin-Client/Plugin/releases)

**The backbone of the Moonfin ecosystem.** A Jellyfin server plugin used by every client that provides:

- **Jellyfin Web & Mobile UI** - Injects the Moonfin experience (media bar, custom details screen, navigation bar, and more) directly into Jellyfin Web and the Mobile App — no separate client needed
- **Cross-Client Settings Sync** - Per-user preferences with device profiles (desktop, mobile, TV) sync across all Moonfin clients automatically
- **Jellyseerr/Seerr Proxy** - Authenticated reverse proxy so clients can integrate Seerr or Jellyseerr without CORS or cookie issues
- **Admin Configuration** - Server-wide default settings, shared API keys for MDBList/TMDB, and centralized Jellyseerr configuration

> **Note:** The plugin is optional for the Jellyfin Web/Mobile experience but **required** for Android TV, Tizen, webOS, and Roku clients' Seerr/Jellyseerr integreation and strongly recommended for settings sync.

## Available Clients

### [Android TV / Fire TV](https://github.com/Moonfin-Client/AndroidTV-FireTV/) 
[![Release](https://img.shields.io/github/release/Moonfin-Client/AndroidTV-FireTV.svg)](https://github.com/Moonfin-Client/AndroidTV-FireTV/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/AndroidTV-FireTV/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/AndroidTV-FireTV/releases) 

**The flagship Moonfin client** for Android TV, Nvidia Shield, and Fire TV devices.

**Platform Highlights:**
- Profile-aware Featured Media Bar with auto-refresh on profile switch
- OTA updates with automatic installation
- Optimized for 10-foot TV viewing

**Supported:** Android TV 6.0+, Nvidia Shield, Fire TV/Stick, Chromecast with Google TV, Google Streamer

---

### [Smart TV — Samsung (Tizen) & LG (webOS)](https://github.com/Moonfin-Client/Smart-TV/) 
[![Release](https://img.shields.io/github/release/Moonfin-Client/Smart-TV.svg)](https://github.com/Moonfin-Client/Smart-TV/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Smart-TV/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/Smart-TV/releases)

**A unified Smart TV client** built with the Enact/Sandstone framework. A single shared codebase powers both Samsung and LG platforms with native video pipelines tuned for each.

**Platform Highlights:**
- Hardware-accelerated video via Samsung AVPlay (Tizen) and Starfish/HTML5 (webOS)
- Automatic screensaver after 90s to prevent burn-in
- Customizable backdrop blur and media bar opacity with sliders
- Dynamic accent color theming
- Trickplay preview thumbnails and media segment skipping
- Live TV with EPG and DVR recordings
- Seerr and Jellyseerr integration via the [Moonfin Plugin](https://github.com/Moonfin-Client/Plugin)

**Supported:** Samsung Smart TVs (Tizen 4.0+, 2018+), LG Smart TVs (webOS 4.0+, 2018+)

---

### [Roku](https://github.com/Moonfin-Client/Roku/) 
[![Release](https://img.shields.io/github/release/Moonfin-Client/Roku.svg)](https://github.com/Moonfin-Client/Roku/releases) [![github](https://img.shields.io/github/downloads/Moonfin-Client/Roku/total?logo=github&label=Downloads)](https://github.com/Moonfin-Client/Roku/releases) 

**The first and only Roku client with Jellyseerr support!**

**Platform Highlights:**
- Modern pill-shaped navigation bar styling
- Updated On Screen Display for the media player with modernized icon set
- Lightweight and optimized for Roku hardware

**Supported:** Roku OS 9.1+ (2018+), Roku TV, Streaming Stick, Ultra, Express

---

### 🚧 Coming Soon
- **Moonfin for tvOS** - Enhanced experience for Apple TV devices

## Installation & Setup

Each client has its own installation method:

- **Android TV / Fire TV:** Download APK from releases and sideload (Android 6.0+)
- **Roku:** Download ZIP package from releases and sideload via developer mode (Roku OS 9.1+)
- **Samsung TV (Tizen):** Download WGT from [Smart-TV releases](https://github.com/Moonfin-Client/Smart-TV/releases) and install via [Samsung Jellyfin Installer](https://github.com/PatrickSt1991/Samsung-Jellyfin-Installer) or Tizen Studio (Tizen 4.0+)
- **LG TV (webOS):** Download IPK from [Smart-TV releases](https://github.com/Moonfin-Client/Smart-TV/releases) and install via webOS Dev Manager or developer mode (webOS 4.0+)
- **Jellyfin Web & Mobile:** Install the [Moonfin Plugin](https://github.com/Moonfin-Client/Plugin) on your Jellyfin server — no separate client download needed

For detailed installation instructions, visit the specific client or plugin repository.

### Moonfin Plugin Setup

The [Moonfin Plugin](https://github.com/Moonfin-Client/Plugin) enhances all clients and is the only way to get Moonfin on Jellyfin Web and Mobile:

1. In Jellyfin Dashboard → Administration → Plugins → Repositories, add:
   - **Name:** `Moonfin`
   - **URL:** `https://raw.githubusercontent.com/Moonfin-Client/Plugin/refs/heads/master/manifest.json`
2. Go to Catalog → find **Moonfin** → Install
3. Restart Jellyfin
4. For the Web UI, also install the [File Transformation](https://github.com/IAmParadox27/jellyfin-plugin-file-transformation) plugin

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
- All the contributors to the upstream Jellyfin projects

Special thanks to everyone who has supported Moonfin development through donations and feedback!

## License

Moonfin clients inherit the licenses of their respective upstream projects:
- Android TV / Fire TV: GPL v2
- Roku: GPL v2
- Smart TV (Tizen & webOS): MPL 2.0
- Plugin: GPL v3

See individual repositories for specific licensing information.

---

<p align="center">
   <i>Moonfin is not affiliated with the Jellyfin project. It is an independent fork focused on enhanced user experiences.</i>
</p>
