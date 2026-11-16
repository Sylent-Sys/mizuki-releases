# Mizuki v2026.11.4 (Stable)

Released: 2026-11-16 | Build: 26111619

## Fixed
- **In-App Auto-Updater (Android Split-per-ABI):** Fixed update evaluation logic to prioritize CalVer comparison over internal build numbers, ensuring Android `arm64-v8a` devices correctly receive release updates despite Gradle ABI offsets.
- **Android Scoped Storage (POSIX Direct I/O):** Added `MANAGE_EXTERNAL_STORAGE` declaration and redirected default storage to app-specific external storage (`/Android/data/com.sylentsys.mizuki.app/files/torrents`), resolving POSIX `EPERM (os error 1)` file write errors in the Rust media engine.

## Changed & Improved
- **Storage Diagnostics & Runtime Permissions:** Added runtime storage permission prompts in Settings and Setup Wizard when selecting custom download locations outside the Android app sandbox.
- **Media Engine Resilience:** Hardened storage directory initialization on Android 11+ to ensure uninterrupted torrent streaming and downloads.

---

## Downloads & SHA-256 Checksums

### Windows (64-bit)
- **Installer:** [Mizuki-Setup-2026.11.4.exe](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.4/Mizuki-Setup-2026.11.4.exe) (~32.1 MB)
  - `sha256: 14f7a4177afe90392dae51d88cf5869db81f773f4d0032098a9121141b9fce13`
  - Unversioned alias: `Mizuki-Setup-x64.exe` (`sha256: 14f7a4177afe90392dae51d88cf5869db81f773f4d0032098a9121141b9fce13`)
- **Portable Archive:** [Mizuki-Windows-x64-2026.11.4.zip](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.4/Mizuki-Windows-x64-2026.11.4.zip) (~43.4 MB)
  - `sha256: 3bdf79d56db8e79ff0baedf46f36b3d0391f30820bc33b0f9508c2601c20085f`

### Android (Split per ABI / Android 10+)
- **arm64-v8a:** [Mizuki-Android-arm64-v8a-2026.11.4.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.4/Mizuki-Android-arm64-v8a-2026.11.4.apk) (~48.9 MB)
  - `sha256: 0f800d91083a43b3e418f0b38318c616c65b8da1fbc84c482a6d3e3fddf47436`
- **armeabi-v7a:** [Mizuki-Android-armeabi-v7a-2026.11.4.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.4/Mizuki-Android-armeabi-v7a-2026.11.4.apk) (~42.3 MB)
  - `sha256: 9ee5a5c942cd5b390f37f473875b7915c89194a06ecb00bce7629b7ca9a2eee0`
- **x86_64:** [Mizuki-Android-x86_64-2026.11.4.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.4/Mizuki-Android-x86_64-2026.11.4.apk) (~54.8 MB)
  - `sha256: 0705f8cd04d7011d2f6e7e8d65094b355a23acfd3137f614a507aa4d4f112bdd`

---

### Legal & Compliance Notice
Mizuki is an open-source, neutral media player and BitTorrent client. It does not host, provide, index, or distribute any copyrighted media content or torrent metadata out of the box. Users are solely responsible for the content they choose to stream or download.
