# Mizuki Changelog

All notable user-facing changes to Mizuki will be documented in this file.

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
