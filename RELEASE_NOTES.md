# Mizuki v2026.11.3 (Stable)

Released: 2026-11-16 | Build: 26111618

## Added
- **Mizuki Design System 1.0:** Unified typography, responsive paddings, rounded borders, and standardized UI components (`MizukiBadge`, `MizukiButton`, `MizukiCard`, `MizukiDialog`) across Adaptive Shell, Airing Calendar, Settings, and Torrent Client screens.
- **Theme Consistency & Contrast:** Polished color token mappings and improved readability across all 4 built-in palettes (Blackout OLED, Whiteout, Catppuccin, and Dracula).

## Fixed
- **Windows Exit Freeze & Deadlock Prevention:** Resolved triple-deadlock race condition during video player teardown on Windows by making player destruction asynchronous, properly detaching event listeners, and ensuring clean tray controller shutdown.

## Changed & Improved
- **Player Diagnostics & Lifecycle:** Added safe lifecycle disposal boundaries for `media_kit` libmpv texture controllers on desktop to guarantee instant, clean application exit without background hangs.

---

## Downloads & SHA-256 Checksums

### Windows (64-bit)
- **Installer:** [Mizuki-Setup-2026.11.3.exe](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.3/Mizuki-Setup-2026.11.3.exe) (~32.1 MB)
  - `sha256: 401aa713a69a88358f89ed37dd4c0fac9b959d314cbca1571e0aa3c2f6b5d3d7`
  - Unversioned alias: `Mizuki-Setup-x64.exe` (`sha256: 401aa713a69a88358f89ed37dd4c0fac9b959d314cbca1571e0aa3c2f6b5d3d7`)
- **Portable Archive:** [Mizuki-Windows-x64-2026.11.3.zip](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.3/Mizuki-Windows-x64-2026.11.3.zip) (~43.4 MB)
  - `sha256: f33272c40c4fdcf449f8bacea91039fcfd682391a2a1ac051bdf8e8bba07577d`

### Android (Split per ABI / Android 10+)
- **arm64-v8a:** [Mizuki-Android-arm64-v8a-2026.11.3.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.3/Mizuki-Android-arm64-v8a-2026.11.3.apk) (~48.9 MB)
  - `sha256: ffb202ebd4f4d57e50935a7c5ad5bb282beb30bc9c852dfbbba1d537484c7355`
- **armeabi-v7a:** [Mizuki-Android-armeabi-v7a-2026.11.3.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.3/Mizuki-Android-armeabi-v7a-2026.11.3.apk) (~42.3 MB)
  - `sha256: ae15ff153ae99d0b02a35071bf457fbd6fb3231bb672ec572c2f3e45c32c3416`
- **x86_64:** [Mizuki-Android-x86_64-2026.11.3.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.3/Mizuki-Android-x86_64-2026.11.3.apk) (~54.8 MB)
  - `sha256: f3cdde13da3b5d49375e3752a9f4c81191d6d567491aa14b2fb1caf03f1952ac`

---

### Legal & Compliance Notice
Mizuki is an open-source, neutral media player and BitTorrent client. It does not host, provide, index, or distribute any copyrighted media content or torrent metadata out of the box. Users are solely responsible for the content they choose to stream or download.
