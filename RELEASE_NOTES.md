# Mizuki v2026.11.2 (Stable)

Released: 2026-11-16 | Build: 26111610

## Added
- **In-App Auto-Updater:** Added **Settings > App & Updates** with a **Stable / Beta** channel selector, current version badge, and a one-click **Check for Updates** workflow with an interactive update dialog.
- **Windows Inno Setup Installer:** Automated packaging into an installer (`Mizuki-Setup-2026.11.2.exe` and `Mizuki-Setup-x64.exe`) featuring the official Mizuki emblem, Start Menu entry, optional Desktop shortcut toggle, and clean uninstallation.
- **Android APK Installer Integration:** Added native Android `FileProvider` and package installation intent handling for direct in-app APK upgrades on Android 10+.
- **Portable Windows Archive & Checksum Manifest:** Added portable ZIP distribution and automated SHA-256 verification across all release artifacts in `releases.json`.

## Changed
- **Streaming & Media Playback:** Instant Rust-powered BitTorrent playback, right-click video context menu (audio tracks, ASS/SSA subtitles, aspect ratio, screenshots), video debanding shader, and Debrid cloud acceleration via Real-Debrid and TorBox.
- **Discovery & Ecosystem:** AniList OAuth auto-scrobble tracking, seasonal airing calendar with My List filtering, studio-grade Torrent Swarm Inspector, and 4 dark/light themes (Blackout OLED, Whiteout, Catppuccin, Dracula).
- **Security & Storage:** Built-in Cloudflare DNS-over-HTTPS encrypted resolution (Jaringan & Privasi DNS), custom storage partition picker, Windows minimize-to-tray background seeding, and clean Win32 version metadata compatibility for CalVer builds.

---

## Downloads & SHA-256 Checksums

### Windows (64-bit)
- **Installer:** [Mizuki-Setup-2026.11.2.exe](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.2/Mizuki-Setup-2026.11.2.exe) (~32.1 MB)
  - `sha256: 838222477d6d0b99d91066007e2b746367f37749838756a33b48fc65575be9bf`
  - Unversioned alias: `Mizuki-Setup-x64.exe` (`sha256: 838222477d6d0b99d91066007e2b746367f37749838756a33b48fc65575be9bf`)
- **Portable Archive:** [Mizuki-Windows-x64-2026.11.2.zip](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.2/Mizuki-Windows-x64-2026.11.2.zip) (~43.4 MB)
  - `sha256: 541db49c65c747105978f50be9f16923e124353a4d1e5d09ba2358adf052ea38`

### Android (Split per ABI / Android 10+)
- **arm64-v8a:** [Mizuki-Android-arm64-v8a-2026.11.2.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.2/Mizuki-Android-arm64-v8a-2026.11.2.apk) (~48.9 MB)
  - `sha256: ca87e04f5e66f473185798e2c6786c3543fe93978d5e80b4f74b676436d57b7a`
- **armeabi-v7a:** [Mizuki-Android-armeabi-v7a-2026.11.2.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.2/Mizuki-Android-armeabi-v7a-2026.11.2.apk) (~42.2 MB)
  - `sha256: f61890c350658a474f8292e98c7b94305272813e2939487fa83fc7a604f4b93e`
- **x86_64:** [Mizuki-Android-x86_64-2026.11.2.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.2/Mizuki-Android-x86_64-2026.11.2.apk) (~54.8 MB)
  - `sha256: 660d856a6c4894bfa2a55d1d52c6f231545bfaf1f1246d505a747b3cf97f4834`

---

### Legal & Compliance Notice
Mizuki is an open-source, neutral media player and BitTorrent client. It does not host, provide, index, or distribute any copyrighted media content or torrent metadata out of the box. Users are solely responsible for the content they choose to stream or download.
