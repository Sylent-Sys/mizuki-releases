# Mizuki v2026.11.2 (Stable)

Released: 2026-11-16 | Build: 26111610

## Added
- **Android Split-per-ABI APK Distribution:** Releases are now packaged and distributed into dedicated architecture APKs (`arm64-v8a`, `armeabi-v7a`, `x86_64`), reducing download sizes to ~42–54 MB (down from ~92 MB monolithic APK).
- **In-App Architecture Detection for Auto-Updater:** Enhanced `UpdateChecker` on Android to query device CPU ABIs (`supportedAbis`) and automatically download the optimal native APK package for the user's device architecture.

## Changed & Improved
- **Build Artifact Hygiene & Pruning:** Automated cleanup of stale build outputs (`dist/`, `jniLibs/`, and intermediate Flutter outputs) prior to packaging to ensure clean, reproducible distribution bundles.
- **Multi-ABI Checksum Manifest:** Updated `releases.json` schema to include structured multi-ABI checksums and direct download endpoints for all Android architectures.

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
