# Mizuki Changelog

All notable user-facing changes to Mizuki will be documented in this file.

## v2026.11.0 (2026-11-15) - Stable

Released: 2026-11-15 | Build: 26111523

## Added
- **In-App Auto-Updater:** Added **Settings > App & Updates** with a **Stable / Beta** channel selector, current version badge, and a one-click **Check for Updates** workflow with an interactive update dialog.
- **Windows Inno Setup Installer:** Automated packaging into an installer (`Mizuki-Setup-2026.11.0.exe` and `Mizuki-Setup-x64.exe`) featuring the official Mizuki emblem, Start Menu entry, optional Desktop shortcut toggle, and clean uninstallation.
- **Android APK Installer Integration:** Added native Android `FileProvider` and package installation intent handling for direct in-app APK upgrades on Android 10+.
- **Portable Windows Archive & Checksum Manifest:** Added portable ZIP distribution and automated SHA-256 verification across all release artifacts in `releases.json`.

## Changed
- **Streaming & Media Playback:** Instant Rust-powered BitTorrent playback, right-click video context menu (audio tracks, ASS/SSA subtitles, aspect ratio, screenshots), video debanding shader, and Debrid cloud acceleration via Real-Debrid and TorBox.
- **Discovery & Ecosystem:** AniList OAuth auto-scrobble tracking, seasonal airing calendar with My List filtering, studio-grade Torrent Swarm Inspector, and 4 dark/light themes (Blackout OLED, Whiteout, Catppuccin, Dracula).
- **Security & Storage:** Built-in Cloudflare DNS-over-HTTPS encrypted resolution, custom storage partition picker, Windows minimize-to-tray background seeding, and clean Win32 version metadata compatibility for CalVer builds.
