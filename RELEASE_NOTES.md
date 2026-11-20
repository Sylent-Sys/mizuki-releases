# Mizuki v2026.11.8 (Stable)

Released: 2026-11-20 | Build: 26112007

## Fixed
- **Android 16 Video Playback Stability:** Fixed a video player crash on Android 16 devices during video startup, background switching, and back navigation by switching Android hardware decoding to surface-safe mode and stopping playback cleanly before closing the player.
- **Better Direct Web Stream Support:** Improved playback compatibility for web-embedded video links, including packed player pages, nested embeds, and malformed link parameters, while showing a clear error message if a host cannot be played directly.
- **Prevented Direct Stream Dropouts:** Removed an overly short download timeout on proxied direct and cloud streams so long episodes play smoothly without cutting off after 15 seconds.
- **Cleaner Player Buffering Indicator:** Hid the buffering spinner when a playback error is shown and updated its status label for direct and cloud streams.

---

## Downloads & SHA-256 Checksums

### Windows (64-bit)
- **Installer:** [Mizuki-Setup-2026.11.8.exe](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.8/Mizuki-Setup-2026.11.8.exe) (~32.7 MB)
  - `sha256: 17f8f8fa25088ac7d76d3ff49aa291c9a73a63dd3e9fb21aa93a3abb24fd2bfe`
  - Unversioned alias: `Mizuki-Setup-x64.exe` (`sha256: 17f8f8fa25088ac7d76d3ff49aa291c9a73a63dd3e9fb21aa93a3abb24fd2bfe`)
- **Portable Archive:** [Mizuki-Windows-x64-2026.11.8.zip](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.8/Mizuki-Windows-x64-2026.11.8.zip) (~44.5 MB)
  - `sha256: f13d09d35d0b035f6de206e9e4879aab34201f0fff995c11ca9c86ad5bbbb554`

### Android (Split per ABI / Android 10+)
- **arm64-v8a:** [Mizuki-Android-arm64-v8a-2026.11.8.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.8/Mizuki-Android-arm64-v8a-2026.11.8.apk) (~50.8 MB)
  - `sha256: 3daa5c0f7d35462d6509b3440590273c1e885a762ce52abfc1934af1ef02580a`
- **armeabi-v7a:** [Mizuki-Android-armeabi-v7a-2026.11.8.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.8/Mizuki-Android-armeabi-v7a-2026.11.8.apk) (~44.2 MB)
  - `sha256: 53ccb680771273d8ec30c01f66ce4d63b51d331ed18b31d498857e107918b36e`
- **x86_64:** [Mizuki-Android-x86_64-2026.11.8.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.8/Mizuki-Android-x86_64-2026.11.8.apk) (~56.6 MB)
  - `sha256: 1b9287621186a367e45faad3214e797577d77b36dbd21e2a3ea157a92b0d0659`

---

### Legal & Compliance Notice
Mizuki is an open-source, neutral media player and BitTorrent client. It does not host, provide, index, or distribute any copyrighted media content or torrent metadata out of the box. Users are solely responsible for the content they choose to stream or download.
