# Mizuki v2026.11.5 (Stable)

Released: 2026-11-17 | Build: 26111716

## Added
- **Progressive Disclosure Settings:** Settings screen now features expandable/collapsible sections and category filters to reduce cognitive load, prioritizing user benefits over technical implementation jargon.
- **Concurrent Source Search & Live Streaming:** Media source plugin searching now runs concurrently with real-time streaming results, an honest progress indicator (`X/Y finished · N found`), and a responsive cancel button.

## Fixed
- **Plugin Persistence & Migration (Data Loss Prevention):** Decoupled media source plugin storage from disposable streaming cache (`torrents`) into dedicated persistent app storage, with idempotent migration on startup to prevent plugins from disappearing across updates.
- **Android In-Place Update Support:** Configured a persistent release signing key for production Android APK builds to prevent signature mismatches and forced uninstalls during updates.
- **Windows Uninstaller Data Safety:** Scoped Inno Setup uninstaller rules to purge only temporary streaming cache files, preserving user-installed plugins and configuration.
- **Android Subtitle Font Rendering:** Updated libass fallback font configuration with a unified OFL-licensed typeface, eliminating tofu/missing glyph boxes on complex subtitle tracks.

## Changed & Improved
- **QRIS Payment Experience:** Refined banking and e-wallet brand presentation and added platform-aware actions ("Save to Gallery" on Android/iOS, "Copy QR Code" on Windows Desktop).
- **Design System Consistency (MDS 1.0):** Standardized input fields, buttons, and segmented controls to a uniform 10px corner radius (`MizukiRadius.md`).

---

## Downloads & SHA-256 Checksums

### Windows (64-bit)
- **Installer:** [Mizuki-Setup-2026.11.5.exe](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.5/Mizuki-Setup-2026.11.5.exe) (~32.9 MB)
  - `sha256: 4f4424a6df7f87a51e43860387a0f86f50d10b9d4e87559d964510e701eea6a5`
  - Unversioned alias: `Mizuki-Setup-x64.exe` (`sha256: 4f4424a6df7f87a51e43860387a0f86f50d10b9d4e87559d964510e701eea6a5`)
- **Portable Archive:** [Mizuki-Windows-x64-2026.11.5.zip](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.5/Mizuki-Windows-x64-2026.11.5.zip) (~44.6 MB)
  - `sha256: cd119c5e7b879e4812d03f6ffba9c1ba8bf8a799f05b0efa406e2236ae119000`

### Android (Split per ABI / Android 10+)
- **arm64-v8a:** [Mizuki-Android-arm64-v8a-2026.11.5.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.5/Mizuki-Android-arm64-v8a-2026.11.5.apk) (~50.2 MB)
  - `sha256: 78c904c278328a14232b63cdaddab5cbe3ced99b61bf305bdfca00f16ca8d556`
- **armeabi-v7a:** [Mizuki-Android-armeabi-v7a-2026.11.5.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.5/Mizuki-Android-armeabi-v7a-2026.11.5.apk) (~43.5 MB)
  - `sha256: c0ffd40053fdf098fb9c5b31bff4f08a62b1d4a529f2c0a7493040541f186625`
- **x86_64:** [Mizuki-Android-x86_64-2026.11.5.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.5/Mizuki-Android-x86_64-2026.11.5.apk) (~56 MB)
  - `sha256: 76358e0f2d59b2e1d5614be937ce23f29cb52bc47aff7ef9ad15e8aed7890f48`

---

### Legal & Compliance Notice
Mizuki is an open-source, neutral media player and BitTorrent client. It does not host, provide, index, or distribute any copyrighted media content or torrent metadata out of the box. Users are solely responsible for the content they choose to stream or download.
