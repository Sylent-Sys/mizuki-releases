# Mizuki v2026.11.5 (Stable)

Released: 2026-11-17 | Build: 26111716

## Added
- **Streamlined Collapsible Settings:** Redesigned the Settings screen with collapsible sections and category filters so options are easier to scan and understand.
- **Live Concurrent Source Search:** Add-on searches now run in parallel with live incoming results, a real-time progress counter (`X/Y finished · N found`), and an instant cancel button.

## Changed & Improved
- **Improved QRIS Payment Experience:** Refined bank and e-wallet branding and added platform-aware actions ("Save to Gallery" on Android and "Copy QR Code" on Windows).
- **Consistent UI Corner Styling:** Standardized corner rounding across text inputs, buttons, and segmented controls for a more cohesive look.

## Fixed
- **Protected User Add-ons Across Updates:** Moved user-installed media source plugins out of the temporary streaming cache into dedicated persistent storage with automatic migration, preventing add-ons from disappearing across updates.
- **Seamless In-Place Android Updates:** Switched production Android releases to a consistent app signature so future updates install directly over existing installations without requiring an uninstall.
- **Safer Windows Uninstaller:** Scoped Windows cleanup to temporary streaming cache files so user-installed add-ons and preferences remain safe.
- **Complete Android Subtitle Font Support:** Replaced the bundled Android subtitle fallback font with a broader Unicode typeface, eliminating missing-character boxes (tofu) on stylized subtitles.

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
