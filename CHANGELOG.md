# Mizuki Changelog

All notable user-facing changes to Mizuki will be documented in this file.

## v2026.11.0 (Initial Release Candidate)

### Streaming & Playback
- **Instant Torrent Streaming:** Stream anime torrents in real-time with zero wait time using the embedded Rust `librqbit` engine and local HTTP 206 range server.
- **Advanced Context Menu:** Right-click desktop menu and mobile quick sheet for seamless audio track switching (Sub/Dub), subtitle selection, video debanding shader, and playback speed.
- **Debrid Cloud Acceleration:** Direct high-speed streaming via Real-Debrid and TorBox for Mizuki PRO Gold members.

### Discovery & Ecosystem
- **AniList Sync & Auto-Scrobble:** Realtime watch progress synchronization with your AniList account.
- **Airing Calendar:** Monthly simulcast broadcast schedule with "My list" filter.
- **Torrent Client Dashboard:** Studio-grade BitTorrent swarm monitoring (DHT/PEX/LSD/NAT-PMP protocol status, peer table, and speeds).
- **Theming Engine:** Four built-in themes: Blackout (OLED), Whiteout, Catppuccin, and Dracula.
- **DNS-over-HTTPS Bawaan:** Cloudflare DoH to bypass ISP DNS hijacking without third-party VPNs.
