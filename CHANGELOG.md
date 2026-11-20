# Mizuki Changelog

All notable user-facing changes to Mizuki will be documented in this file.

## v2026.11.7 (2026-11-20) - Stable

Released: 2026-11-20 | Build: 26112006

## Added
- **More Ways to Stream:** Watch episodes from direct web streams, Usenet, standard torrents, or cloud services like Real-Debrid and TorBox (Gold)—all from a single source picker.
- **Skip Intros & Outros (Bronze+):** Added a "Skip Opening / Ending" button on the video player with chapter markers on the timeline bar, plus an optional Auto-Skip switch in Settings.
- **Watch Together with Friends:** Host a private Watch Party room (Bronze+) or join any friend's room for free with a 6-character code to keep playback in sync, complete with live chat and emoji reactions.
- **Richer Episode Details:** Episode lists now show full episode titles, story summaries, air dates, runtimes, filler badges, and preview thumbnails in both Grid and Compact List views.
- **Continue Watching & Mini-Player:** Added a "Continue Watching" section on the Discover tab to jump right back into unfinished episodes, plus a docked Mini-Player so you can browse the app without stopping your video.
- **Ambient Video Lighting & Timeline Previews:** Added an Ambient Mode toggle that projects a soft glow around the video player, along with thumbnail previews when scrubbing across the timeline bar.
- **Smarter Search Filters:** Filter anime by multiple genres and tags at once, alongside format, airing status, season, and release year on the Search screen.
- **Linux Desktop Support:** Mizuki is now available natively on Linux desktops with full window and system tray support matching the Windows experience.

## Fixed
- **Smoother Direct Web Streaming:** Improved compatibility with direct video streams so multi-quality playlists, audio tracks, and subtitles load reliably without playback stalls.
- **Automatic Stream Recovery:** The player now automatically retries when a stream server briefly hiccups or slows down, reducing unexpected buffering interruptions.

## Changed & Improved
- **Faster & More Stable App Engine:** Upgraded the core app framework for smoother animations, crisper menus, and better overall stability across Windows, Linux, and Android.

## v2026.11.6 (2026-11-18) - Stable

Released: 2026-11-18 | Build: 26111800

## Added
- **Subscription Checkout Details Card:** Added a dedicated transaction details card beneath the checkout QR view, showing the order reference, plan name, tax itemization, and service fee in a clean dark slate container.

## Fixed
- **Choice Chip Duration Selection Reflow:** Disabled active checkmark indicator on subscription duration chips (`showCheckmark: false`) in ProScreen to prevent unintended text shift and layout reflow.
- **Order Verification Settlement Matching:** Refined backend verification matching to ensure seamless transaction status updates upon confirmation.

## Changed & Improved
- **Checkout Modal UI Polish:** Polished dark slate layout spacing, typography hierarchy, and platform-specific action button alignment.
- **Release Manifest Consistency:** Streamlined automated release packaging and bullet-point parsing for in-app updater manifests across stable update channels.

## v2026.11.5 (2026-11-17) - Stable

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

## v2026.11.4 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111619

## Fixed
- **In-App Auto-Updater (Android Split-per-ABI):** Fixed update evaluation logic to prioritize CalVer comparison over internal build numbers, ensuring Android `arm64-v8a` devices correctly receive release updates despite Gradle ABI offsets.
- **Android Scoped Storage (POSIX Direct I/O):** Added `MANAGE_EXTERNAL_STORAGE` declaration and redirected default storage to app-specific external storage (`/Android/data/com.sylentsys.mizuki.app/files/torrents`), resolving POSIX `EPERM (os error 1)` file write errors in the Rust media engine.

## Changed & Improved
- **Storage Diagnostics & Runtime Permissions:** Added runtime storage permission prompts in Settings and Setup Wizard when selecting custom download locations outside the Android app sandbox.
- **Media Engine Resilience:** Hardened storage directory initialization on Android 11+ to ensure uninterrupted torrent streaming and downloads.

## v2026.11.3 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111618

## Added
- **Mizuki Design System 1.0:** Unified typography, responsive paddings, rounded borders, and standardized UI components (`MizukiBadge`, `MizukiButton`, `MizukiCard`, `MizukiDialog`) across Adaptive Shell, Airing Calendar, Settings, and Torrent Client screens.
- **Theme Consistency & Contrast:** Polished color token mappings and improved readability across all 4 built-in palettes (Blackout OLED, Whiteout, Catppuccin, and Dracula).

## Fixed
- **Windows Exit Freeze & Deadlock Prevention:** Resolved triple-deadlock race condition during video player teardown on Windows by making player destruction asynchronous, properly detaching event listeners, and ensuring clean tray controller shutdown.

## Changed & Improved
- **Player Diagnostics & Lifecycle:** Added safe lifecycle disposal boundaries for `media_kit` libmpv texture controllers on desktop to guarantee instant, clean application exit without background hangs.

## v2026.11.2 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111610

## Added
- **Android Split-per-ABI APK Distribution:** Releases are now packaged and distributed into dedicated architecture APKs (`arm64-v8a`, `armeabi-v7a`, `x86_64`), reducing download sizes to ~42–54 MB (down from ~92 MB monolithic APK).
- **In-App Architecture Detection for Auto-Updater:** Enhanced `UpdateChecker` on Android to query device CPU ABIs (`supportedAbis`) and automatically download the optimal native APK package for the user's device architecture.

## Changed & Improved
- **Build Artifact Hygiene & Pruning:** Automated cleanup of stale build outputs (`dist/`, `jniLibs/`, and intermediate Flutter outputs) prior to packaging to ensure clean, reproducible distribution bundles.
- **Multi-ABI Checksum Manifest:** Updated `releases.json` schema to include structured multi-ABI checksums and direct download endpoints for all Android architectures.

## v2026.11.1 (2026-11-16) - Stable

Released: 2026-11-16 | Build: 26111608

## Added
- **In-App QRIS Checkout & Dynamic Pricing Catalog:** Added dynamic Silver and Gold membership packages with an interactive in-app QRIS payment dialog featuring live countdown, automatic payment verification, QR PNG export, and instant license activation.

## Fixed
- **Android ASS/SSA Subtitle Font Rendering:** Bundled `DroidSansFallback.ttf` for Android `libass` playback so stylized and fallback subtitle characters render cleanly on mobile devices.

## Changed & Improved
- **Player Diagnostics & Release Pipeline:** Restricted verbose libmpv/libass font logs to debug builds and improved release changelog formatting consistency.

## v2026.11.0 (2026-11-15) - Stable

Released: 2026-11-15 | Build: 26111523

## Added
- **In-App Auto-Updater:** Added **Settings > App & Updates** with a **Stable / Beta** channel selector, current version badge, and a one-click **Check for Updates** workflow with an interactive update dialog.
- **Windows Inno Setup Installer:** Automated packaging into an installer (`Mizuki-Setup-2026.11.0.exe` and `Mizuki-Setup-x64.exe`) featuring the official Mizuki emblem, Start Menu entry, optional Desktop shortcut toggle, and clean uninstallation.
- **Android APK Installer Integration:** Added native Android `FileProvider` and package installation intent handling for direct in-app APK upgrades on Android 10+.
- **Portable Windows Archive & Checksum Manifest:** Added portable ZIP distribution and automated SHA-256 verification across all release artifacts in `releases.json`.

## Changed
- **Streaming & Media Playback:** Instant Rust-powered BitTorrent playback, right-click video context menu (audio tracks, ASS/SSA subtitles, aspect ratio, screenshots), video debanding shader, and Debrid cloud acceleration via Real-Debrid and TorBox.
- **Discovery & Ecosystem:** AniList OAuth auto-scrobble tracking, seasonal airing calendar with My List filtering, studio-grade Torrent Swarm Inspector, and 4 dark/light themes (Blackout OLED, Whiteout, Catppuccin, Dracula).
- **Security & Storage:** Built-in Cloudflare DNS-over-HTTPS encrypted resolution (Jaringan & Privasi DNS), custom storage partition picker, Windows minimize-to-tray background seeding, and clean Win32 version metadata compatibility for CalVer builds.
