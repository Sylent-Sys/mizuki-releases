# Mizuki Changelog

All notable user-facing changes to Mizuki will be documented in this file.

## v2026.11.8 (2026-11-20) - Stable

Released: 2026-11-20 | Build: 26112007

### Fixed
- **Android 16 Video Playback Stability:** Fixed a video player crash on Android 16 devices during video startup, background switching, and back navigation by switching Android hardware decoding to surface-safe mode and stopping playback cleanly before closing the player.
- **Better Direct Web Stream Support:** Improved playback compatibility for web-embedded video links, including packed player pages, nested embeds, and malformed link parameters, while showing a clear error message if a host cannot be played directly.
- **Prevented Direct Stream Dropouts:** Removed an overly short download timeout on proxied direct and cloud streams so long episodes play smoothly without cutting off after 15 seconds.
- **Cleaner Player Buffering Indicator:** Hid the buffering spinner when a playback error is shown and updated its status label for direct and cloud streams.

## v2026.11.7 (2026-11-20) - Stable

Released: 2026-11-20 | Build: 26112006

### Added
- **More Ways to Stream:** Watch episodes from direct web streams, Usenet, standard torrents, or cloud services like Real-Debrid and TorBox (Gold)—all from a single source picker.
- **Skip Intros & Outros (Bronze+):** Added a "Skip Opening / Ending" button on the video player with chapter markers on the timeline bar, plus an optional Auto-Skip switch in Settings.
- **Watch Together with Friends:** Host a private Watch Party room (Bronze+) or join any friend's room for free with a 6-character code to keep playback in sync, complete with live chat and emoji reactions.
- **Richer Episode Details:** Episode lists now show full episode titles, story summaries, air dates, runtimes, filler badges, and preview thumbnails in both Grid and Compact List views.
- **Continue Watching & Mini-Player:** Added a "Continue Watching" section on the Discover tab to jump right back into unfinished episodes, plus a docked Mini-Player so you can browse the app without stopping your video.
- **Ambient Video Lighting & Timeline Previews:** Added an Ambient Mode toggle that projects a soft glow around the video player, along with thumbnail previews when scrubbing across the timeline bar.
- **Smarter Search Filters:** Filter anime by multiple genres and tags at once, alongside format, airing status, season, and release year on the Search screen.
- **Linux Desktop Support (Source Build):** Added native Linux desktop window and system tray support matching the Windows experience for users building from source; prebuilt Linux packages will follow in a future release.

### Changed & Improved
- **Faster & More Stable App Engine:** Upgraded the core app framework for smoother animations, crisper menus, and better overall stability across Windows, Linux, and Android.

### Fixed
- **Smoother Direct Web Streaming:** Improved compatibility with direct video streams so multi-quality playlists, audio tracks, and subtitles load reliably without playback stalls.
- **Automatic Stream Recovery:** The player now automatically retries when a stream server briefly hiccups or slows down, reducing unexpected buffering interruptions.

## v2026.11.6 (2026-11-18) - Stable

Released: 2026-11-18 | Build: 26111800

### Added
- **Subscription Checkout Details Card:** Added a transaction summary card beneath the checkout QR view displaying your order reference, selected plan, tax breakdown, and service fee in a clean dark container.

### Changed & Improved
- **Checkout Modal Polish:** Refined spacing, typography hierarchy, and platform-specific action button alignment inside the checkout dialog.

### Fixed
- **Duration Selector Layout Shift:** Fixed subscription duration buttons shifting width and reflowing when selected on the PRO screen.
- **Reliable Payment Confirmation:** Improved automatic order verification so completed QRIS payments activate more consistently.

## v2026.11.5 (2026-11-17) - Stable

Released: 2026-11-17 | Build: 26111716

### Added
- **Streamlined Collapsible Settings:** Redesigned the Settings screen with collapsible sections and category filters so options are easier to scan and understand.
- **Live Concurrent Source Search:** Add-on searches now run in parallel with live incoming results, a real-time progress counter (`X/Y finished · N found`), and an instant cancel button.

### Changed & Improved
- **Improved QRIS Payment Experience:** Refined bank and e-wallet branding and added platform-aware actions ("Save to Gallery" on Android and "Copy QR Code" on Windows).
- **Consistent UI Corner Styling:** Standardized corner rounding across text inputs, buttons, and segmented controls for a more cohesive look.

### Fixed
- **Protected User Add-ons Across Updates:** Moved user-installed media source plugins out of the temporary streaming cache into dedicated persistent storage with automatic migration, preventing add-ons from disappearing across updates.
- **Seamless In-Place Android Updates:** Switched production Android releases to a consistent app signature so future updates install directly over existing installations without requiring an uninstall.
- **Safer Windows Uninstaller:** Scoped Windows cleanup to temporary streaming cache files so user-installed add-ons and preferences remain safe.
- **Complete Android Subtitle Font Support:** Replaced the bundled Android subtitle fallback font with a broader Unicode typeface, eliminating missing-character boxes (tofu) on stylized subtitles.

## v2026.11.4 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111619

### Changed & Improved
- **Guided Custom Folder Permissions:** Added runtime storage permission prompts in Settings and the Setup Wizard when choosing a custom download location on Android.
- **More Reliable Android 11+ Storage Setup:** Strengthened storage directory initialization on Android 11 and newer for uninterrupted streaming and downloads.

### Fixed
- **Android Update Detection:** Fixed an issue where some Android devices failed to detect newly published app updates.
- **Android Storage Write Errors:** Added full storage access support for custom folders and switched the default download folder to a safe app-owned storage directory on Android 11+, eliminating file write permission errors during playback.

## v2026.11.3 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111618

### Added
- **Refreshed Unified Interface:** Introduced consistent typography, responsive spacing, and unified badges, buttons, cards, and dialogs across navigation, Airing Calendar, Settings, and Transfers screens.
- **Improved Theme Contrast:** Refined color contrast and text readability across all four built-in themes (Blackout OLED, Whiteout, Catppuccin, and Dracula).

### Changed & Improved
- **Cleaner Desktop Player Shutdown:** Hardened video player cleanup when closing desktop windows so the app exits cleanly without leaving background processes behind.

### Fixed
- **Windows Exit Freeze:** Fixed a freeze that could occur when closing Mizuki on Windows while a video player or system tray session was active.

## v2026.11.2 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111610

### Added
- **Smaller Per-Device Android Downloads:** Android releases are now packaged separately by device architecture (`arm64-v8a`, `armeabi-v7a`, and `x86_64`), cutting typical download sizes nearly in half (~42–55 MB instead of ~92 MB).
- **Automatic Device Architecture Detection:** The in-app updater on Android now automatically detects your device architecture and downloads the right APK package for your phone or tablet.

## v2026.11.1 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111608

### Added
- **In-App QRIS Checkout & Dynamic Plans:** Added Silver and Gold membership plans with an interactive in-app QRIS payment dialog featuring a live countdown timer, automatic payment verification, QR image export, and instant activation.

### Fixed
- **Android Subtitle Font Rendering:** Bundled a fallback subtitle font on Android so stylized ASS/SSA subtitles and non-Latin characters display properly on mobile devices.

## v2026.11.0 (2026-11-15) - Stable

Released: 2026-11-15 | Build: 26111523

### Added
- **In-App Auto-Updater:** Added **Settings > App & Updates** with release channel selection, a current version badge, and one-click **Check for Updates** with an interactive update dialog.
- **Windows Installer & Portable Archive:** Added a Windows desktop installer with Start Menu integration, optional Desktop shortcut, and clean uninstallation, alongside a portable ZIP archive with SHA-256 verification.
- **Direct Android In-App Upgrades:** Added native Android package installer handoff so updates downloaded in-app can be installed directly on Android 10+.

### Changed & Improved
- **Instant Media Playback:** Fast BitTorrent streaming with right-click/mobile player controls (audio tracks, ASS/SSA subtitles, aspect ratio, screenshots), video debanding, and optional Debrid cloud acceleration via Real-Debrid and TorBox.
- **Discovery & Ecosystem:** AniList OAuth auto-scrobble tracking, seasonal airing calendar with My List filtering, detailed Torrent Swarm Inspector, and four built-in themes (Blackout OLED, Whiteout, Catppuccin, and Dracula).
- **Network Privacy & Storage:** Built-in Cloudflare DNS-over-HTTPS (Encrypted DNS), custom download folder selection, and Windows minimize-to-tray background seeding.
