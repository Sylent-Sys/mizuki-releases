# Mizuki Changelog

All notable user-facing changes to Mizuki will be documented in this file.

## v2026.11.2 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111610

## Added
- **Android Split-per-ABI APK Distribution:** Releases are now packaged and distributed into dedicated architecture APKs (`arm64-v8a`, `armeabi-v7a`, `x86_64`), reducing download sizes to ~42–54 MB (down from ~92 MB monolithic APK).
- **In-App Architecture Detection for Auto-Updater:** Enhanced `UpdateChecker` on Android to query device CPU ABIs (`supportedAbis`) and automatically download the optimal native APK package for the user's device architecture.

## Changed & Improved
- **Build Artifact Hygiene & Pruning:** Automated cleanup of stale build outputs (`dist/`, `jniLibs/`, and intermediate Flutter outputs) prior to packaging to ensure clean, reproducible distribution bundles.
- **Multi-ABI Checksum Manifest:** Updated `releases.json` schema to include structured multi-ABI checksums and direct download endpoints for all Android architectures.

## v2026.11.1 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111608

## Added
- **In-App QRIS Checkout & Dynamic Pricing Catalog:** Added dynamic Silver and Gold membership packages with an interactive in-app QRIS payment dialog featuring live countdown, automatic payment verification, QR PNG export, and instant license activation.

## Fixed
- **Android ASS/SSA Subtitle Font Rendering:** Bundled `DroidSansFallback.ttf` for Android `libass` playback so stylized and fallback subtitle characters render cleanly on mobile devices.

## Changed & Improved
- **Player Diagnostics & Release Pipeline:** Restricted verbose libmpv/libass font logs to debug builds and improved release changelog formatting consistency.

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
- **Security & Storage:** Built-in Cloudflare DNS-over-HTTPS encrypted resolution (Jaringan & Privasi DNS), custom storage partition picker, Windows minimize-to-tray background seeding, and clean Win32 version metadata compatibility for CalVer builds.
