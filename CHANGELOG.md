# Mizuki Changelog

All notable user-facing changes to Mizuki will be documented in this file.

## v2026.11.4 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111619

### Changed & Improved
- **Guided Custom Folder Permissions:** Added runtime storage permission prompts in Settings and the Setup Wizard when choosing a custom download location on Android.
- **More Reliable Android 11+ Storage Setup:** Strengthened storage directory initialization on Android 11 and newer for uninterrupted streaming and downloads.

### Fixed
- **Android Update Detection:** Fixed an issue where some Android devices failed to detect newly published app updates.
- **Android Storage Write Errors:** Added full storage access support for custom folders and switched the default download folder to a safe app-owned storage directory on Android 11+, eliminating file write permission errors during playback.

## v2026.11.3 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111618

### Added
- **Refreshed Unified Interface:** Introduced consistent typography, responsive spacing, and unified badges, buttons, cards, and dialogs across navigation, Airing Calendar, Settings, and Transfers screens.
- **Improved Theme Contrast:** Refined color contrast and text readability across all four built-in themes (Blackout OLED, Whiteout, Catppuccin, and Dracula).

### Changed & Improved
- **Cleaner Desktop Player Shutdown:** Hardened video player cleanup when closing desktop windows so the app exits cleanly without leaving background processes behind.

### Fixed
- **Windows Exit Freeze:** Fixed a freeze that could occur when closing Mizuki on Windows while a video player or system tray session was active.

## v2026.11.2 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111610

### Added
- **Smaller Per-Device Android Downloads:** Android releases are now packaged separately by device architecture (`arm64-v8a`, `armeabi-v7a`, and `x86_64`), cutting typical download sizes nearly in half (~42–55 MB instead of ~92 MB).
- **Automatic Device Architecture Detection:** The in-app updater on Android now automatically detects your device architecture and downloads the right APK package for your phone or tablet.

## v2026.11.1 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111608

### Added
- **In-App QRIS Checkout & Dynamic Plans:** Added Silver and Gold membership plans with an interactive in-app QRIS payment dialog featuring a live countdown timer, automatic payment verification, QR image export, and instant activation.

### Fixed
- **Android Subtitle Font Rendering:** Bundled a fallback subtitle font on Android so stylized ASS/SSA subtitles and non-Latin characters display properly on mobile devices.

## v2026.11.0 (2026-11-15) - Stable

Released: 2026-11-15 | Build: 26111523

### Added
- **In-App Auto-Updater:** Added **Settings > App & Updates** with release channel selection, a current version badge, and one-click **Check for Updates** with an interactive update dialog.
- **Windows Installer & Portable Archive:** Added a Windows desktop installer with Start Menu integration, optional Desktop shortcut, and clean uninstallation, alongside a portable ZIP archive with SHA-256 verification.
- **Direct Android In-App Upgrades:** Added native Android package installer handoff so updates downloaded in-app can be installed directly on Android 10+.

### Changed & Improved
- **Instant Media Playback:** Fast BitTorrent streaming with right-click/mobile player controls (audio tracks, ASS/SSA subtitles, aspect ratio, screenshots), video debanding, and optional Debrid cloud acceleration via Real-Debrid and TorBox.
- **Discovery & Ecosystem:** AniList OAuth auto-scrobble tracking, seasonal airing calendar with My List filtering, detailed Torrent Swarm Inspector, and four built-in themes (Blackout OLED, Whiteout, Catppuccin, and Dracula).
- **Network Privacy & Storage:** Built-in Cloudflare DNS-over-HTTPS (Encrypted DNS), custom download folder selection, and Windows minimize-to-tray background seeding.
