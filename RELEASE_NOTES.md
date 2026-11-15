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
- **Security & Storage:** Built-in Cloudflare DNS-over-HTTPS encrypted resolution (Jaringan & Privasi DNS), custom storage partition picker, Windows minimize-to-tray background seeding, and clean Win32 version metadata compatibility for CalVer builds.

---

## Downloads & SHA-256 Checksums

### Windows (64-bit)
- **Installer:** [Mizuki-Setup-2026.11.0.exe](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.0/Mizuki-Setup-2026.11.0.exe) (~30.8 MB)
  - `sha256: 1fb47c855987f5ec0eef3854ccbbd9c1f2ecbe080d06539bde5da999d244aea6`
  - Unversioned alias: `Mizuki-Setup-x64.exe` (`sha256: 1fb47c855987f5ec0eef3854ccbbd9c1f2ecbe080d06539bde5da999d244aea6`)
- **Portable Archive:** [Mizuki-Windows-x64-2026.11.0.zip](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.0/Mizuki-Windows-x64-2026.11.0.zip) (~41.7 MB)
  - `sha256: a91c7686c70866e8b5d49f8f819056b2a3363ada89a83966a42d8cf8c0556d07`

### Android (arm64-v8a / Android 10+)
- **Release APK:** [Mizuki-Android-arm64-2026.11.0.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.0/Mizuki-Android-arm64-2026.11.0.apk) (~90.2 MB)
  - `sha256: d33d00bf7e364ef765b78ddf8508c2531dfee2dad2161a7e4e2551b859b967d3`

---

### Legal & Compliance Notice
Mizuki is an open-source, neutral media player and BitTorrent client. It does not host, provide, index, or distribute any copyrighted media content or torrent metadata out of the box. Users are solely responsible for the content they choose to stream or download.
