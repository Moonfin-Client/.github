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
- **Upstream compatibility** - Full compatibility with any Jellyfin server (no server modifications needed)
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
-  **Automatic Updates** - Built-in update checker with in-app notifications

## Available Clients

### [Android TV / Fire TV](https://github.com/Moonfin-Client/AndroidTV-FireTV/) [![Release](https://img.shields.io/github/release/Moonfin-Client/AndroidTV-FireTV.svg)](https://github.com/Moonfin-Client/AndroidTV-FireTV/releases)

**The flagship Moonfin client** for Android TV, Nvidia Shield, and Fire TV devices.

**Platform Highlights:**
- Profile-aware Featured Media Bar with auto-refresh on profile switch
- OTA updates with automatic installation
- Optimized for 10-foot TV viewing

**Supported:** Android TV 6.0+, Nvidia Shield, Fire TV/Stick, Chromecast with Google TV, Google Streamer

---

### [Roku](https://github.com/Moonfin-Client/Roku/) [![Release](https://img.shields.io/github/release/Moonfin-Client/Roku.svg)](https://github.com/Moonfin-Client/Roku/releases)

**The first and only Roku client with Jellyseerr support!**

**Platform Highlights:**
- Modern pill-shaped navigation bar styling
- Updated On Screen Display for the media player with modernized icon set
- Lightweight and optimized for Roku hardware

**Supported:** Roku OS 9.1+ (2018+), Roku TV, Streaming Stick, Ultra, Express

---

### [Samsung TV (Tizen)](https://github.com/Moonfin-Client/Tizen/) [![Release](https://img.shields.io/github/release/Moonfin-Client/Tizen.svg)](https://github.com/Moonfin-Client/Tizen/releases)


**Platform Highlights:**
- Automatic screensaver after 90s to prevent burn-in
- Customizable backdrop blur and media bar opacity with sliders
- Dynamic accent color theming


**Supported:** Samsung Smart TVs (Tizen 4+, 2016+). Tizen 5.5+ recommended.

---

### [LG TV (WebOS)](https://github.com/Moonfin-Client/WebOS/) [![Release](https://img.shields.io/github/release/Moonfin-Client/WebOS.svg)](https://github.com/Moonfin-Client/WebOS/releases)

**Optimized for LG Magic Remote** with theme music and accent color customization.

**Platform Highlights:**
- Automatic screensaver after 90s to prevent burn-in
- Customizable backdrop blur and media bar opacity with sliders
- Dynamic accent color theming
- Optimized for LG Magic Remote

  
**Supported:** LG Smart TVs (WebOS 3.0+, 2016+)

---

### 🚧 Coming Soon
- **Moonfin for tvOS** - Enhanced experience for Apple TV devices

## Installation & Setup

Each client has its own installation method:

- **Android TV / Fire TV:** Download APK from releases and sideload (Android 6.0+)
- **Roku:** Download ZIP package from releases and sideload via developer mode (Roku OS 9.1+)
- **Samsung TV (Tizen):** Download WGT package from releases and install via [Samsung Jellyfin Installer](https://github.com/PatrickSt1991/Samsung-Jellyfin-Installer) or Tizen Studio (Tizen 4+)
- **LG TV (WebOS):** Download IPK package from releases and install via webOS Dev Manager or developer mode (WebOS 3.0+)

For detailed installation instructions, visit the specific client repository.

### Optional: Jellyseerr Setup

To enable media discovery and requesting in Moonfin clients:

1. Install and configure [Jellyseerr](https://jellyseerr.dev/) on your network
2. In Moonfin settings, navigate to the Jellyseerr section
3. Enter your Jellyseerr server URL and authenticate with your Jellyfin credentials
4. Start discovering and requesting content!

## Community & Support

- **Upstream Jellyfin:** [jellyfin.org](https://jellyfin.org)
- **Buy Me a Coffee:** [buymeacoffee.com/moonfin](https://www.buymeacoffee.com/moonfin)
- **Issues & Feature Requests:** Submit in the specific client repository
- **Discussions:** Available in each client repository

## Contributing

We welcome contributions! Moonfin is built on the hard work of the Jellyfin community, and we aim to contribute improvements back upstream where appropriate.

If you're interested in contributing:
1. Check out the specific client README for build instructions
2. Review open issues and discussions
3. For changes that should go upstream, please coordinate with Jellyfin maintainers
4. Follow the existing code style and conventions for each platform

## Credits

Moonfin builds upon:
- **Jellyfin Project** - The amazing open-source media server and clients
- **MakD's Jellyfin-Media-Bar** - Inspiration for the media bar feature
- All the contributors to the upstream Jellyfin projects

Special thanks to everyone who has supported Moonfin development through donations and feedback!

## License

Moonfin clients inherit the licenses of their respective upstream projects:
- Android TV / Fire TV: GPL v2
- Roku: GPL v2
- Samsung TV (Tizen): MPL 2.0
- LG TV (WebOS): MPL 2.0

See individual client repositories for specific licensing information.

---

<p align="center">
   <i>Moonfin is not affiliated with the Jellyfin project. It is an independent fork focused on enhanced user experiences.</i>
</p>
