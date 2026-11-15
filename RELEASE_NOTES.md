# Mizuki v2026.11.0 (Stable)

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

---

## Downloads & SHA-256 Checksums

### Windows (64-bit)
- **Installer:** [Mizuki-Setup-2026.11.0.exe](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.0/Mizuki-Setup-2026.11.0.exe) (~30.8 MB)
  - `sha256: e65a1d3629db5e009a04aef56e1424c1d6f8cb718cadf4ac6c795ae978280540`
  - Unversioned alias: `Mizuki-Setup-x64.exe` (`sha256: e65a1d3629db5e009a04aef56e1424c1d6f8cb718cadf4ac6c795ae978280540`)
- **Portable Archive:** [Mizuki-Windows-x64-2026.11.0.zip](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.0/Mizuki-Windows-x64-2026.11.0.zip) (~41.7 MB)
  - `sha256: 63d0b39e966ccfa81661064a593f7f9acd8ed27474c2d8b8098870cf774ac97c`

### Android (arm64-v8a / Android 10+)
- **Release APK:** [Mizuki-Android-arm64-2026.11.0.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.0/Mizuki-Android-arm64-2026.11.0.apk) (~90.2 MB)
  - `sha256: 8d8e31cb4cec94ac4f04657780d9fe4120dcb05c36c1609ebe09c72d53645b61`
