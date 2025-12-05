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
- **Jellyseerr Integration** - First-class support for content discovery and requesting (first native Jellyfin clients with Jellyseerr!)
- **Platform-optimized experiences** - Each client is tailored for its specific device type
- **Upstream compatibility** - Full compatibility with any Jellyfin server (no server modifications needed)
- **Open source** - All improvements are available for the community to use and contribute to

## Available Clients

### 📺 [Android TV / Fire TV](https://github.com/Moonfin-Client/AndroidTV-FireTV/)
The flagship Moonfin client for Android TV, Nvidia Shield, and Amazon Fire TV devices.

**Key Features:**
- **Jellyseerr Integration** - Browse trending, popular, and recommended content. Request movies/TV shows in HD or 4K
- **NSFW Content Filtering** - Automatic filtering for family-safe browsing in Jellyseerr (configurable)
- **Profile-aware Media Bar** - Rotating featured content that respects profile permissions and refreshes on profile switch
- **Pre-playback Track Selection** - Choose audio/subtitle tracks before playback starts
- **Enhanced Detail Screens** - Grouped metadata, circular cast photos, taglines, and refined layouts
- **Customizable Toolbar** - Toggle library buttons, shuffle filters, and favorites
- **OTA Updates** - Built-in update checker with automatic installation
- Optimized for 10-foot TV viewing experience

**Latest Release:** [![Release](https://img.shields.io/github/release/Moonfin-Client/AndroidTV-FireTV.svg)](https://github.com/Moonfin-Client/AndroidTV-FireTV/releases)

**Supported Devices:** Android TV (5.0+), Nvidia Shield, Fire TV, Fire Stick, Google TV

---

### 📱 [Roku](https://github.com/Moonfin-Client/Roku/)
Enhanced Jellyfin client for Roku streaming devices - the first and only Roku client with Jellyseerr support!

**Key Features:**
- **Jellyseerr Integration (Beta)** - Browse trending content, request movies/TV shows, track your requests
- **NSFW Content Filtering** - Automatic adult content filtering with TMDB flags and keyword detection
- **Featured Media Bar** - Auto-rotating carousel of 15 random movies/shows with ratings and overview
- **Customizable Toolbar** - Toggle Shuffle, Genres, Favorites buttons. Show/hide library row
- **Pre-playback Track Selection** - Choose audio/subtitle tracks before playback starts
- **Enhanced Navigation** - Quick home/search buttons, genres menu, dynamic library buttons
- **Lazy Loading** - Optimized performance with pagination (100 items per batch)
- **Automatic Update Checker** - Get notified when new versions are available
- Circular cast photos and improved metadata display

**Latest Release:** [![Release](https://img.shields.io/github/release/Moonfin-Client/Roku.svg)](https://github.com/Moonfin-Client/Roku/releases)

**Supported Devices:** All Roku devices (Roku OS 9.0+), Roku TV, Roku Streaming Stick, Roku Ultra, Roku Express

---

### 🚧 Coming Soon
- **Moonfin for tvOS** - Enhanced experience for Apple TV devices
- **Moonfin for LG WebOS** - Native client for LG Smart TVs
- **Moonfin for Tizen OS** - Native client for Samsung Smart TVs

## Installation & Setup

Each client has its own installation method:

- **Android TV / Fire TV:** Download APK from releases and sideload
- **Roku:** Download ZIP package from releases and sideload via developer mode

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

See individual client repositories for specific licensing information.

---

<p align="center">
   <i>Moonfin is not affiliated with the Jellyfin project. It is an independent fork focused on enhanced user experiences.</i>
</p>
