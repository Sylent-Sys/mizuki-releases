# Mizuki Changelog

All notable user-facing changes to Mizuki will be documented in this file.

## v2026.11.14 (2026-11-25) - Stable

Released: 2026-11-25 | Build: 26112513

### Fixed
- **AniList Sign-In on Android:** Fixed an issue where tapping **Connect AniList** on Android could fail to start sign-in after updating or signing out.
- **Clearer Account Sign-In Notices:** Improved account sign-in error messages in Settings so they are easier to understand.

## v2026.11.13 (2026-11-25) - Stable

Released: 2026-11-25 | Build: 26112506

### Added
- **Expanded Media Add-On Compatibility:** Custom add-ons now support subtitle add-ons, HTTP webseed accelerators, Usenet (NZB) sources with optional NNTP server settings, compact repository shortcuts (`gh:` and `npm:`), and parallel episode and seasonal pack discovery.
- **Extension Diagnostics & Update Checker:** Added one-click **Test**, **Test All**, and **Check Updates** controls on the Extensions screen with live online status, response times, diagnostic logs, automatic startup update checks, and compatibility notices.
- **Faster Source Discovery & Live Peer Counts:** Added optional live BitTorrent tracker peer refresh in Network Settings so source lists display current seeder and leecher counts, plus on-demand stream resolution for faster episode searches.

### Changed & Improved
- **Smarter Episode Matching & Source Ranking:** Episode lookups now use richer cross-catalog metadata and absolute episode numbers, highlight recommended and seasonal releases more clearly, show multi-source attribution when several add-ons list the same release, and support `.ico` add-on icons.
- **Better Multi-Theme Contrast & Touch Targets:** Improved text and badge readability across Whiteout, Catppuccin, and Dracula themes and enlarged extension card buttons for easier tapping on touchscreens.
- **Improved Cloud Streaming for Torrent Links:** Torrent file links returned by add-ons can now resolve through enabled Debrid cloud services without falling back to peer-to-peer downloads.

### Fixed
- **Missing Add-On Session Verification Shortcut:** Add-ons that require browser-style host verification now display a direct **Verify Session** button on their card and prefill the host URL automatically.

## v2026.11.12 (2026-11-24) - Stable

Released: 2026-11-24 | Build: 26112407

### Added
- **Premiere Release Dates & Live Episode Countdowns:** Anime detail pages now display the premiere release date in the header, and every episode card shows accurate release dates and live airing countdowns (such as In 23 hours, In 1 week, or 6 days ago) with exact broadcast date and time tooltips.
- **Expanded Episode Previews for Seasonal Anime & Specials:** Added multi-source episode metadata resolution so newly airing seasonal series, OVAs, ONAs, and specials reliably load episode thumbnails, English titles, synopses, community ratings, and runtimes.

### Changed & Improved
- **Cleaner Upcoming Episode Cards & Accurate Numbering:** Upcoming episodes without preview artwork now use a clean, compact card layout without empty placeholder boxes, and mid-season recaps or specials automatically align by air date so episode titles and previews stay matched.

### Fixed
- **Missing Thumbnails & Release Dates on Newly Airing Shows:** Fixed anime detail pages showing blank episode cards with missing titles, thumbnails, and release dates when primary catalog mappings were incomplete.

## v2026.11.11 (2026-11-23) - Stable

Released: 2026-11-23 | Build: 26112317

### Changed & Improved
- **Instant Watch Together Media Sharing:** Creating a Watch Together room while a video is already playing—including direct magnet links or stream URLs—now immediately shares the active video and current timestamp with the room.
- **Automatic Sync for Late-Joining Friends:** Friends who join an active Watch Together room after playback has started now automatically load the host's video and sync straight to the current timestamp.
- **Stronger Watch Together Room Protection:** Watch Together rooms now use longer, harder-to-guess room codes, verify Bronze Pass or higher status when hosting, enforce host-only playback and media controls, and protect room chat against sender impersonation or flooding.
- **Seamless Supporter Pass Continuity:** Prepared supporter pass verification for upcoming security updates so active passes keep working smoothly across Windows and Android without interruption.

### Fixed
- **Watch Together Connection Feedback:** Removed an unresponsive fallback connection state so joining an invalid, expired, or unreachable room now immediately shows a clear status message instead of appearing connected.
- **Consistent Fonts in Settings Inputs:** Fixed text fields and dropdown selectors in Settings so they properly match your selected app theme font.

## v2026.11.10 (2026-11-22) - Stable

Released: 2026-11-22 | Build: 26112222

### Changed & Improved
- **Clearer Episode Progress Bars:** Increased episode watch progress bar height and track contrast across all four themes (Blackout, Whiteout, Catppuccin, Dracula) so partially watched episodes are easy to gauge at a glance.
- **Cleaner In-App Update Notes:** Improved formatting inside the in-app update dialog so release note headings and highlights render cleanly.

### Fixed
- **False Progress Indicator on Episode Cards:** Fixed a decorative line below episode titles that made unwatched, completed, and upcoming episodes look partially watched. Progress bars now appear only on episodes actively in progress with a known duration.
- **Incomplete Update Prompts:** Prevented the in-app updater from prompting to install an update before its downloadable package is ready.

## v2026.11.9 (2026-11-22) - Stable

Released: 2026-11-22 | Build: 26112213

### Added
- **Redesigned Adaptive Stream Source Picker:** Replaced the compact source popup with an adaptive picker tailored to every screen size—a full-screen mobile view with a thumb-friendly bottom filter bar and slide-up Filter, Hosts, and Manual Link sheets, a spacious tablet dialog, and a dual-pane desktop layout with an independent sidebar.
- **Interactive Host Verification (WebView):** Added an in-app **Verify in WebView** flow for content providers and direct video hosts that require interactive browser verification, automatically remembering site sessions across restarts, retrying your search or playback, and letting you clear site cookies per add-on in Extensions.
- **Adaptive Stream Stats HUD & Transfer Tracking:** Updated the in-player Stats HUD (`H`) to show live streaming throughput, buffer-ahead duration, and real-time playback details (resolution, FPS, codecs, hardware decoder, dropped frames, and buffered cache) for Direct, HLS, and Debrid cloud streams, while also showing active non-torrent streams on the Transfers screen and navigation badge.
- **Richer Add-on Settings & External Subtitles:** Add-on option dialogs now display native toggles, dropdown menus, number fields, and masked API key/token inputs, alongside automatic loading of external subtitle tracks from web content providers, full movie and batch source lookups, and authenticated stream playback.

### Changed & Improved
- **Faster Seeking & Smoother Buffering:** Pre-loads the start and end of torrent video files so timeline seeking responds immediately, prefetches upcoming video data ahead of playback, expands the player's seekable memory buffer (128 MB forward / 64 MB backward), and merges rapid step-seek taps (`±5s` / `±10s`) into a single smooth jump with instant on-screen feedback.
- **Parallel Source Search & Faster Repository Installs:** Source searches now run concurrently across all enabled add-ons and stream results into the picker as providers respond, with instant **Stop** cancellation when closing or refreshing, while multi-add-on repositories now install scripts in parallel.
- **Cleaner Source Rows & Last-Used Highlighting:** Unified source cards across mobile and desktop with compact quality and origin badges, pinned **Last used** highlighting (including a fallback row when a cached source is not in the current results), and instant **Direct Magnet Detected** quick-stream when pasting a magnet link into the filter box.

### Fixed
- **Mobile Stream Picker Layout & Overflows:** Fixed cramped source lists and layout overflows on narrow mobile screens when resume bars, cached sources, and host verification prompts appeared together, ensuring safe-area padding, keyboard-aware bottom controls, and clean contrast across all four themes (Blackout, Whiteout, Catppuccin, Dracula).
- **Direct & Cloud Stream Telemetry:** Fixed Direct HTTP, HLS, and Debrid streams showing placeholder `0 B/s` speeds, `0 peers`, or `100% (Seed)` status in the Stats HUD, Transfers screen, and Android foreground notifications.
- **Search Cancellation & Picker Cleanup:** Fixed lingering background search activity after cancellation or errors and improved cleanup when closing and reopening the manual link sheet.

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
