# Mizuki v2026.11.13 (Stable)

Released: 2026-11-25 | Build: 26112506

## Added
- **Expanded Media Add-On Compatibility:** Custom add-ons now support subtitle add-ons, HTTP webseed accelerators, Usenet (NZB) sources with optional NNTP server settings, compact repository shortcuts (`gh:` and `npm:`), and parallel episode and seasonal pack discovery.
- **Extension Diagnostics & Update Checker:** Added one-click **Test**, **Test All**, and **Check Updates** controls on the Extensions screen with live online status, response times, diagnostic logs, automatic startup update checks, and compatibility notices.
- **Faster Source Discovery & Live Peer Counts:** Added optional live BitTorrent tracker peer refresh in Network Settings so source lists display current seeder and leecher counts, plus on-demand stream resolution for faster episode searches.

## Changed & Improved
- **Smarter Episode Matching & Source Ranking:** Episode lookups now use richer cross-catalog metadata and absolute episode numbers, highlight recommended and seasonal releases more clearly, show multi-source attribution when several add-ons list the same release, and support `.ico` add-on icons.
- **Better Multi-Theme Contrast & Touch Targets:** Improved text and badge readability across Whiteout, Catppuccin, and Dracula themes and enlarged extension card buttons for easier tapping on touchscreens.
- **Improved Cloud Streaming for Torrent Links:** Torrent file links returned by add-ons can now resolve through enabled Debrid cloud services without falling back to peer-to-peer downloads.

## Fixed
- **Missing Add-On Session Verification Shortcut:** Add-ons that require browser-style host verification now display a direct **Verify Session** button on their card and prefill the host URL automatically.

---

## Downloads & SHA-256 Checksums

### Windows (64-bit)
- **Installer:** [Mizuki-Setup-2026.11.13.exe](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.13/Mizuki-Setup-2026.11.13.exe) (~33.2 MB)
  - `sha256: e64281dcbeda59570418c9efebdb1794e0e37df57fa67ead68540a2b2083074b`
  - Unversioned alias: `Mizuki-Setup-x64.exe` (`sha256: e64281dcbeda59570418c9efebdb1794e0e37df57fa67ead68540a2b2083074b`)
- **Portable Archive:** [Mizuki-Windows-x64-2026.11.13.zip](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.13/Mizuki-Windows-x64-2026.11.13.zip) (~44.4 MB)
  - `sha256: 32bd1942bc3688c03231925774d438455416bd90a9c64d2b7143254713cf83e3`

### Android (Split per ABI / Android 10+)
- **arm64-v8a:** [Mizuki-Android-arm64-v8a-2026.11.13.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.13/Mizuki-Android-arm64-v8a-2026.11.13.apk) (~52.9 MB)
  - `sha256: 41dcdde489eab626a02e9ee031774f9e4baf0bf52c2a554844827be05119cd86`
- **armeabi-v7a:** [Mizuki-Android-armeabi-v7a-2026.11.13.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.13/Mizuki-Android-armeabi-v7a-2026.11.13.apk) (~45.9 MB)
  - `sha256: 7e5fb511b21f6948498d118ab2f69775af39b7566ef3d1ff66200dd2434c144b`
- **x86_64:** [Mizuki-Android-x86_64-2026.11.13.apk](https://github.com/Sylent-Sys/mizuki-releases/releases/download/v2026.11.13/Mizuki-Android-x86_64-2026.11.13.apk) (~59.1 MB)
  - `sha256: b62e237f4c1459f2114e14818eea6f69b508facb4228076096510de9309181e5`

---

### Legal & Compliance Notice
Mizuki is a free-to-use, neutral media player and BitTorrent client. It does not host, provide, index, or distribute any copyrighted media content or torrent metadata out of the box. Users are solely responsible for the content they choose to stream or download.
