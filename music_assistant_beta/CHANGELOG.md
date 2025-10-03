# [2.7.0.b0] - 03.10.2025

## What’s Changed

### Server 2.7.0.b0

## :bow: Thanks to our contributors

Special thanks to the following contributors who helped with this release:

@ChrisBkt, @MarvinSchenkel, @MedievalApple, @OzGav, @TheJulianJES, @benklop, @dependabot[bot], @fmunkes, @marcelveldt, @maximmaxim345, @music-assistant-machine and [dependabot[bot]](https://github.com/apps/dependabot)

## Full Changelog

- #2470 - Fix release drafter workflow `latest` value (@TheJulianJES)
- #2461 - Revert "mypy fixes for webserver.py" (@MarvinSchenkel)

## 🐛 Bugfixes

- #2469 - Fix playergroup migration (@marcelveldt)
- #2468 - Fix current track not updating correctly (@marcelveldt)
- #2466 - Various follow up bugfixes regarding the players refactor (@marcelveldt)
- #2464 - YTMusic: Limit dynamic playlist to avoid memory leak (@MarvinSchenkel)
- #2444 - Various Playergroup fixes (@marcelveldt)
- #2455 - Fix 403 error on podcast playback (@OzGav)
- #2433 - Several improvements to the Smartfades feature (@marcelveldt)
- #2429 - More grouping fixes after the player refactor (@maximmaxim345)
- #2425 - gpodder/ itunes/ rssfeed: fix bad header for certain podcasts (@fmunkes)

## 🚀 Features

- #2419 - Add DI.fm radio network provider (@benklop)
- #2457 - Smart fades tweaks (@MarvinSchenkel)
- #2435 - Podcastfeed Handle images no longer at URL (@OzGav)
- #2432 - Adding alexa language config value (@ChrisBkt)
- #2442 - Few smart fades fixes (@MarvinSchenkel)
- #2441 - Adjust smart fades filters from testing (@maximmaxim345)
- #2433 - Several improvements to the Smartfades feature (@marcelveldt)
- #2411 - Add Internet Archive Provider (@OzGav)
- #2407 - Add Smart fades feature (@MarvinSchenkel)
- #2430 - Refactor caching (@marcelveldt)
- #2348 - Add Resonate Provider (@maximmaxim345)
- #2410 - Add Audiobook Support to Spotify provider (@OzGav)
- #2332 - Add (Roku) Media Assistant provider (@MedievalApple)

## 🧰 Maintenance

- #2471 - frontend-2.16.4 (@music-assistant-machine)
- #2467 - frontend-2.16.3 (@music-assistant-machine)
- #2444 - Various Playergroup fixes (@marcelveldt)
- #2459 - frontend-2.16.2 (@music-assistant-machine)
- #2437 - mypy fixes for webserver.py (@OzGav)
- #2449 - mypy fixes for TuneIn (@OzGav)
- #2436 - mypy fixes for Spotify provider (@OzGav)
- #2438 - mypy fixes for Deezer (@OzGav)
- #2439 - mypy fixes for webserver helper (@OzGav)
- #2440 - Remove unsupported library methods (@OzGav)
- #2431 - Add or update stage key in manifest.json (@OzGav)
- #2428 - Update Provider descriptions (@OzGav)
- #2430 - Refactor caching (@marcelveldt)

### Frontend 2.16.4

## 🐛 Bugfixes

- #1164 - Some very small fixes and tweaks after beta testing (@marcelveldt)

## ⬆️ Dependencies

### Server

<details>
<summary>3 changes</summary>

- #2454 - Chore(deps): Bump syrupy from 4.9.1 to 5.0.0 (@[dependabot[bot]](https://github.com/apps/dependabot))
- #2447 - Chore(deps): Bump xmltodict from 0.14.2 to 1.0.2 (@[dependabot[bot]](https://github.com/apps/dependabot))
- #2443 - Chore(deps): Bump docker/login-action from 3.5.0 to 3.6.0 (@[dependabot[bot]](https://github.com/apps/dependabot))
</details>

### Frontend



# [2.7.0 BETA 0] - 02.10.2025

# Music Assistant 2.7.0 BETA 0 Release Notes 🎵

**⚠️ IMPORTANT: Beta Release Notice ⚠️**

This marks the beginning of a new beta cycle for Music Assistant 2.7.0, featuring significant architectural changes, refactoring, and new functionality. **Please ensure you have a complete backup of your Music Assistant data before updating**. 

Due to the extensive changes in this release, we strongly recommend testing in a non-production environment first or at least have a backup ready of your previous version before updating (so you can easily restore to a working situation if something may break for your situation). If you encounter any issues, please report them on our [GitHub Issues](https://github.com/music-assistant/support/issues) or join the discussion on [Discord](https://discord.gg/kaVm8hGpne).

---

## 🎵 New Providers and Features

### New Providers

• **Radio Paradise** - High-quality commercial-free radio with excellent curation by [@OzGav](https://github.com/OzGav) in [#2295](https://github.com/music-assistant/server/pull/2295)

• **Genius Lyrics** - Enhanced lyrics metadata provider by [@robert-alfaro](https://github.com/robert-alfaro) in [#2337](https://github.com/music-assistant/server/pull/2337)

• **Podcast Index** - Access to the comprehensive Podcast Index directory by [@OzGav](https://github.com/OzGav) in [#2350](https://github.com/music-assistant/server/pull/2350)

• **ARD Audiothek** - German public radio's podcast and audio content by [@jfeil](https://github.com/jfeil) in [#2229](https://github.com/music-assistant/server/pull/2229)

• **Resonate** - Initial support for the Resonate (working title) streaming protocol by [@maximmaxim345](https://github.com/maximmaxim345) in [#2348](https://github.com/music-assistant/server/pull/2348)

• **Internet Archive** - Access to audio content from the Internet Archive by [@OzGav](https://github.com/OzGav) in [#2411](https://github.com/music-assistant/server/pull/2411)

• **Media Assistant (Roku)** - Support for Roku devices via Media Assistant by [@MedievalApple](https://github.com/MedievalApple) in [#2332](https://github.com/music-assistant/server/pull/2332)

### Major New Features

• **DSP Presets** - Save and apply custom DSP configurations by [@math625f](https://github.com/math625f) in [#2309](https://github.com/music-assistant/server/pull/2309)

• **Smart Fades** - Initial implementation of the Smart Fades feature: Intelligent crossfading between tracks by [@MarvinSchenkel](https://github.com/MarvinSchenkel) in [#2407](https://github.com/music-assistant/server/pull/2407) with improvements by [@marcelveldt](https://github.com/marcelveldt) in [#2433](https://github.com/music-assistant/server/pull/2433)

• **Enhanced Spotify Support** - Added podcast and audiobook support by [@OzGav](https://github.com/OzGav) in [#2349](https://github.com/music-assistant/server/pull/2349) and [#2410](https://github.com/music-assistant/server/pull/2410)

• **Customizable Announcement Chimes** - Configure custom chime URLs for announcements by [@marcelveldt](https://github.com/marcelveldt) in [#2403](https://github.com/music-assistant/server/pull/2403)

• **Library Sync Controls** - New config options to control how library items are synced by [@marcelveldt](https://github.com/marcelveldt) in [#2405](https://github.com/music-assistant/server/pull/2405)

### Frontend changes

This update brings the first step in the overhaul of the UI !
In next iterations we will go ahead and improve more of the UI, making it easier to use and setup.
Amazing work @Algram @stvncode and @trisweb 

• [#1074](https://github.com/music-assistant/frontend/pull/1074) - DSP Presets (@math625f)

• [#1064](https://github.com/music-assistant/frontend/pull/1064) - Added 'Now Playing' styling to currently playing album/artist/track in all view modes (@uptimeZERO)

• [#1061](https://github.com/music-assistant/frontend/pull/1061) - Add interactive breadcrumb navigation to Browse section (@stvncode)

• [#1082](https://github.com/music-assistant/frontend/pull/1082) - fix: DSP editing bugs with multiple players (@maximmaxim345)

• [#1073](https://github.com/music-assistant/frontend/pull/1073) - Fix: Prevent player cards from collapsing in slider (@FabionRabushja)

• [#1099](https://github.com/music-assistant/frontend/pull/1099) - Podcast multi select menu played / unplayed (@OzGav)

• [#1105](https://github.com/music-assistant/frontend/pull/1105) - Replace mods components (@stvncode)

• [#1080](https://github.com/music-assistant/frontend/pull/1080) - Refactor button component and remove mods (@stvncode)

• [#1107](https://github.com/music-assistant/frontend/pull/1107) - feat(home): ui refresh (@Algram)

• [#1122](https://github.com/music-assistant/frontend/pull/1122) - Improve Multi select favourite (@OzGav)

• [#1146](https://github.com/music-assistant/frontend/pull/1146) - Some small optimizations to config entries (@marcelveldt)

• [#1138](https://github.com/music-assistant/frontend/pull/1138) - Add album types (@OzGav)

• [#1139](https://github.com/music-assistant/frontend/pull/1139) - Hiding the select button in case there's no reason to select items (@robsonke)

• [#1123](https://github.com/music-assistant/frontend/pull/1123) - Fix groups after the player model refactor (@maximmaxim345)

• [#1151](https://github.com/music-assistant/frontend/pull/1151) - Fix mobile toolbar and fonts + players features (@stvncode)

• [#1137](https://github.com/music-assistant/frontend/pull/1137) - Fix lyrics showing timestamps (@OzGav)

• [#1150](https://github.com/music-assistant/frontend/pull/1150) - First iteration of reworking the settings pages: the providers view (@stvncode)

---

## 🐛 Bug Fixes and Enhancements

• **Spotify CDN Fixes** - Resolved CDN issues affecting playback by [@marcelveldt](https://github.com/marcelveldt) in [#2317](https://github.com/music-assistant/server/pull/2317)

• **Spotify Refactor** - Major refactoring and improvements by [@OzGav](https://github.com/OzGav) in [#2329](https://github.com/music-assistant/server/pull/2329)

• **YTMusic Auto-updates** - Automatic dependency updates for stability by [@MarvinSchenkel](https://github.com/MarvinSchenkel) in [#2311](https://github.com/music-assistant/server/pull/2311)

• **SnapCast State Updates** - Fixed broken state updates by [@maximmaxim345](https://github.com/maximmaxim345) in [#2305](https://github.com/music-assistant/server/pull/2305)

• **Audiobook Chapter Sorting** - Sort based on disk number by [@jamiethecat](https://github.com/jamiethecat) in [#2302](https://github.com/music-assistant/server/pull/2302)

• **Album Info Preservation** - Fixed album info being lost for non-library items by [@OzGav](https://github.com/OzGav) in [#2330](https://github.com/music-assistant/server/pull/2330)

• **Podcast Episode Status Sync** - Added played status sync for Spotify podcasts by [@OzGav](https://github.com/OzGav) in [#2408](https://github.com/music-assistant/server/pull/2408)

• **Album Type Support** - Added live and soundtrack album types by [@OzGav](https://github.com/OzGav) in [#2406](https://github.com/music-assistant/server/pull/2406)

• **Podcast Image Handling** - Better handling of missing/broken podcast images by [@OzGav](https://github.com/OzGav) in [#2435](https://github.com/music-assistant/server/pull/2435) and [#2455](https://github.com/music-assistant/server/pull/2455)

• **SoundCloud Recommendations** - Added recommendation support by [@robsonke](https://github.com/robsonke) in [#2275](https://github.com/music-assistant/server/pull/2275)

• **Bluesound Native Grouping** - Native grouping and external source control by [@JoProbst](https://github.com/JoProbst) in [#2359](https://github.com/music-assistant/server/pull/2359)

• **Bluesound multi-zone device Support** - Multi-zone device support via MDNS by [@Cyanogenbot](https://github.com/Cyanogenbot) in [#2358](https://github.com/music-assistant/server/pull/2358)

• **Audiobookshelf JWT Auth** - Modern JWT authorization support by [@fmunkes](https://github.com/fmunkes) in [#2379](https://github.com/music-assistant/server/pull/2379)

• **Audiobookshelf Multi-file Seeking** - Efficient seeking across multi-file audiobooks by [@tsipinakis](https://github.com/tsipinakis) in [#2342](https://github.com/music-assistant/server/pull/2342)

• **Improved Lyrics Availability** - Better lyrics discovery and caching by [@OzGav](https://github.com/OzGav) in [#2357](https://github.com/music-assistant/server/pull/2357)

• **Album Type Inference** - Automatic album type detection for streaming providers by [@OzGav](https://github.com/OzGav) in [#2420](https://github.com/music-assistant/server/pull/2420)

• **Alexa Language Configuration** - Configurable language settings by [@ChrisBkt](https://github.com/ChrisBkt) in [#2432](https://github.com/music-assistant/server/pull/2432)

• **Track Grouping Field** - Expose grouping metadata for tracks by [@cr7pt0gr4ph7](https://github.com/cr7pt0gr4ph7) in [#2373](https://github.com/music-assistant/server/pull/2373)

### Core System Improvements

• **Major Player Controller Refactor** - Complete overhaul of player management architecture by [@marcelveldt](https://github.com/marcelveldt) in [#2249](https://github.com/music-assistant/server/pull/2249)

• **Library Query Improvements** - Fixed random order and improved maintainability by [@maximmaxim345](https://github.com/maximmaxim345) in [#2270](https://github.com/music-assistant/server/pull/2270)

• **Cache Refactoring** - Major caching system improvements by [@marcelveldt](https://github.com/marcelveldt) in [#2430](https://github.com/music-assistant/server/pull/2430)

• **Package Installation Fixes** - Better handling of dynamic package installation by [@marcelveldt](https://github.com/marcelveldt) in [#2318](https://github.com/music-assistant/server/pull/2318) and pip fallback by [@marcelveldt](https://github.com/marcelveldt) in [#2316](https://github.com/music-assistant/server/pull/2316)

• **"This Device" Firefox Fix** - Attempt to fix disappearing/reappearing issues by [@maximmaxim345](https://github.com/maximmaxim345) in [#2271](https://github.com/music-assistant/server/pull/2271)

• **Web Player iOS Support** - Fixed playback issues on iOS devices by [@maximmaxim345](https://github.com/maximmaxim345) in [#2319](https://github.com/music-assistant/server/pull/2319)

• **Invalid Replaygain Handling** - Better handling of invalid replaygain tag values by [@OzGav](https://github.com/OzGav) in [#2282](https://github.com/music-assistant/server/pull/2282)

• **Queue Handling** - Fixed missing file breaks queue by [@OzGav](https://github.com/OzGav) in [#2341](https://github.com/music-assistant/server/pull/2341)

• **Player Settings** - Fixed saving of settings on powered off players by [@maximmaxim345](https://github.com/maximmaxim345) in [#2383](https://github.com/music-assistant/server/pull/2383)

• **Provider Disabling** - Fixed issues when disabling player providers by [@maximmaxim345](https://github.com/maximmaxim345) in [#2388](https://github.com/music-assistant/server/pull/2388)

• **Audiobook Controller Fixes** - Various audiobook-related bug fixes by [@OzGav](https://github.com/OzGav) in [#2412](https://github.com/music-assistant/server/pull/2412)

---

## 🏗️ Technical Changes and Maintenance

<details>
<summary>🔧 Dependency Bumps and Maintenance</summary>

• Bump aiohttp from 3.12.13 to 3.12.15 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2281](https://github.com/music-assistant/server/pull/2281), [#2298](https://github.com/music-assistant/server/pull/2298)

• Bump cryptography from 45.0.4 to 46.0.1 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2276](https://github.com/music-assistant/server/pull/2276), [#2326](https://github.com/music-assistant/server/pull/2326), [#2398](https://github.com/music-assistant/server/pull/2398), [#2418](https://github.com/music-assistant/server/pull/2418)

• Bump mypy from 1.15.0 to 1.18.2 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2284](https://github.com/music-assistant/server/pull/2284), [#2325](https://github.com/music-assistant/server/pull/2325), [#2402](https://github.com/music-assistant/server/pull/2402), [#2417](https://github.com/music-assistant/server/pull/2417)

• Bump ruff from 0.11.13 to 0.12.12 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2285](https://github.com/music-assistant/server/pull/2285), [#2291](https://github.com/music-assistant/server/pull/2291), [#2299](https://github.com/music-assistant/server/pull/2299), [#2323](https://github.com/music-assistant/server/pull/2323), [#2355](https://github.com/music-assistant/server/pull/2355), [#2365](https://github.com/music-assistant/server/pull/2365), [#2386](https://github.com/music-assistant/server/pull/2386)

• Bump async-upnp-client from 0.44.0 to 0.45.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2292](https://github.com/music-assistant/server/pull/2292)

• Bump certifi from 2025.6.15 to 2025.8.3 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2288](https://github.com/music-assistant/server/pull/2288), [#2345](https://github.com/music-assistant/server/pull/2345)

• Bump orjson from 3.10.18 to 3.11.3 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2290](https://github.com/music-assistant/server/pull/2290), [#2344](https://github.com/music-assistant/server/pull/2344), [#2366](https://github.com/music-assistant/server/pull/2366)

• Bump pre-commit from 4.2.0 to 4.3.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2324](https://github.com/music-assistant/server/pull/2324)

• Bump pre-commit-hooks from 5.0.0 to 6.0.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2346](https://github.com/music-assistant/server/pull/2346)

• Bump pytest from 8.4.1 to 8.4.2 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2400](https://github.com/music-assistant/server/pull/2400)

• Bump pytest-cov from 6.2.1 to 7.0.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2401](https://github.com/music-assistant/server/pull/2401)

• Bump syrupy from 4.9.1 to 5.0.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2454](https://github.com/music-assistant/server/pull/2454)

• Bump xmltodict from 0.14.2 to 1.0.2 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2447](https://github.com/music-assistant/server/pull/2447)

• Bump liblistenbrainz from 0.5.6 to 0.6.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2322](https://github.com/music-assistant/server/pull/2322)

• Bump pyblu from 2.0.1 to 2.0.5 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2385](https://github.com/music-assistant/server/pull/2385)

• Bump alexapy from 1.29.5 to 1.29.8 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2371](https://github.com/music-assistant/server/pull/2371)

• Bump ytmusicapi from 1.10.3 to 1.11.1 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2370](https://github.com/music-assistant/server/pull/2370)

• Bump soco from 0.30.10 to 0.30.12 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2368](https://github.com/music-assistant/server/pull/2368), [#2416](https://github.com/music-assistant/server/pull/2416)

• Bump plexapi from 4.17.0 to 4.17.1 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2367](https://github.com/music-assistant/server/pull/2367)

• Bump zeroconf from 0.147.0 to 0.147.2 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2384](https://github.com/music-assistant/server/pull/2384)

• Bump lyricsgenius from 3.6.5 to 3.7.2 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2415](https://github.com/music-assistant/server/pull/2415)

• Bump actions/download-artifact from 4 to 5 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2303](https://github.com/music-assistant/server/pull/2303)

• Bump docker/login-action from 3.4.0 to 3.6.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2297](https://github.com/music-assistant/server/pull/2297), [#2443](https://github.com/music-assistant/server/pull/2443)

• Bump actions/checkout from 4 to 5 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2327](https://github.com/music-assistant/server/pull/2327)

• Bump actions/setup-python from 5.6.0 to 6.0.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2377](https://github.com/music-assistant/server/pull/2377)

• Bump actions/github-script from 7 to 8 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2376](https://github.com/music-assistant/server/pull/2376)

• Bump pypa/gh-action-pypi-publish from 1.12.4 to 1.13.0 by [@dependabot[bot]](https://github.com/dependabot[bot]) in [#2375](https://github.com/music-assistant/server/pull/2375), [#2374](https://github.com/music-assistant/server/pull/2374)

• Add backport pipeline by [@MarvinSchenkel](https://github.com/MarvinSchenkel) in [#2268](https://github.com/music-assistant/server/pull/2268)

• Fix backport pipeline issues by [@MarvinSchenkel](https://github.com/MarvinSchenkel) in [#2272](https://github.com/music-assistant/server/pull/2272), [#2294](https://github.com/music-assistant/server/pull/2294)

• Add CLAUDE.md development guide by [@MarvinSchenkel](https://github.com/MarvinSchenkel) in [#2274](https://github.com/music-assistant/server/pull/2274)

• Add command line server startup instructions by [@tavva](https://github.com/tavva) in [#2396](https://github.com/music-assistant/server/pull/2396)

• Modernise setup script to use uv consistently by [@Crooked-Krokr](https://github.com/Crooked-Krokr) in [#2378](https://github.com/music-assistant/server/pull/2378)

• Adjust funding.yml to OHF by [@marcelveldt](https://github.com/marcelveldt) in [#2267](https://github.com/music-assistant/server/pull/2267)

• Update librespot binaries by [@OzGav](https://github.com/OzGav) in [#2306](https://github.com/music-assistant/server/pull/2306) and [@marcelveldt](https://github.com/marcelveldt) in [#2313](https://github.com/music-assistant/server/pull/2313)

• Use separate ingress TCP site for HA add-on by [@marcelveldt](https://github.com/marcelveldt) in [#2314](https://github.com/music-assistant/server/pull/2314)

• Add helpers to setup aiohttp session by [@marcelveldt](https://github.com/marcelveldt) in [#2308](https://github.com/music-assistant/server/pull/2308)

• Bump models to 1.1.55 by [@marcelveldt](https://github.com/marcelveldt) in [#2397](https://github.com/music-assistant/server/pull/2397)

• Update builtin provider icons by [@OzGav](https://github.com/OzGav) in [#2381](https://github.com/music-assistant/server/pull/2381), [#2380](https://github.com/music-assistant/server/pull/2380)

• Update provider descriptions by [@OzGav](https://github.com/OzGav) in [#2428](https://github.com/music-assistant/server/pull/2428)

• Add stage key in manifest.json by [@OzGav](https://github.com/OzGav) in [#2431](https://github.com/music-assistant/server/pull/2431)

• Remove unsupported library methods by [@OzGav](https://github.com/OzGav) in [#2440](https://github.com/music-assistant/server/pull/2440)

• MyPy fixes across multiple providers by [@OzGav](https://github.com/OzGav) in [#2438](https://github.com/music-assistant/server/pull/2438), [#2436](https://github.com/music-assistant/server/pull/2436), [#2449](https://github.com/music-assistant/server/pull/2449), [#2439](https://github.com/music-assistant/server/pull/2439), [#2437](https://github.com/music-assistant/server/pull/2437)

• Frontend updates: 2.15.3, 2.15.4, 2.16.0, 2.16.1, 2.16.2 by [@music-assistant-machine](https://github.com/music-assistant-machine) in [#2333](https://github.com/music-assistant/server/pull/2333), [#2389](https://github.com/music-assistant/server/pull/2389), [#2422](https://github.com/music-assistant/server/pull/2422), [#2424](https://github.com/music-assistant/server/pull/2424), [#2459](https://github.com/music-assistant/server/pull/2459)

• Disable new PO token generation to avoid warnings by [@MarvinSchenkel](https://github.com/MarvinSchenkel) in [#2334](https://github.com/music-assistant/server/pull/2334)

• Add URL example documentation by [@OzGav](https://github.com/OzGav) in [#2287](https://github.com/music-assistant/server/pull/2287)

• Add caching and fix audiobook podcast mixup by [@OzGav](https://github.com/OzGav) in [#2392](https://github.com/music-assistant/server/pull/2392)

• Refactor Radio Paradise provider by [@OzGav](https://github.com/OzGav) in [#2394](https://github.com/music-assistant/server/pull/2394)

• Fix ARD Audiothek filter iterator by [@jfeil](https://github.com/jfeil) in [#2404](https://github.com/music-assistant/server/pull/2404)

• Fix ARD Audiothek subscriptions and episode ordering by [@jfeil](https://github.com/jfeil) in [#2423](https://github.com/music-assistant/server/pull/2423)

• Fix bad header for certain podcasts by [@fmunkes](https://github.com/fmunkes) in [#2425](https://github.com/music-assistant/server/pull/2425)

• iTunes podcast log improvements by [@fmunkes](https://github.com/fmunkes) in [#2363](https://github.com/music-assistant/server/pull/2363)

• Improve Radio Browser browse implementation by [@OzGav](https://github.com/OzGav) in [#2393](https://github.com/music-assistant/server/pull/2393)

• Smart fades tweaks and adjustments by [@MarvinSchenkel](https://github.com/MarvinSchenkel) in [#2442](https://github.com/music-assistant/server/pull/2442), [#2457](https://github.com/music-assistant/server/pull/2457) and [@maximmaxim345](https://github.com/maximmaxim345) in [#2441](https://github.com/music-assistant/server/pull/2441)

• **XDG Directory Support** - Better data/cache organization following XDG standards by [@jamiethecat](https://github.com/jamiethecat) in [#2304](https://github.com/music-assistant/server/pull/2304)

</details>

---

## 👥 New Contributors

We're thrilled to welcome these amazing new contributors to the Music Assistant community! 🎉

**First-time contributors:**

• [@jamiethecat](https://github.com/jamiethecat) - XDG directory support and audiobook improvements

• [@math625f](https://github.com/math625f) - DSP Presets feature

• [@jeblair](https://github.com/jeblair) - Home Assistant player fixes

• [@tsipinakis](https://github.com/tsipinakis) - Audiobookshelf multi-file seeking

• [@JoProbst](https://github.com/JoProbst) - Bluesound native grouping

• [@robert-alfaro](https://github.com/robert-alfaro) - Genius Lyrics provider

• [@Crooked-Krokr](https://github.com/Crooked-Krokr) - Setup script modernization

• [@jfeil](https://github.com/jfeil) - ARD Audiothek provider

• [@tavva](https://github.com/tavva) - Development documentation

• [@cr7pt0gr4ph7](https://github.com/cr7pt0gr4ph7) - Track grouping field support

• [@MedievalApple](https://github.com/MedievalApple) - Media Assistant (Roku) provider

• [@ChrisBkt](https://github.com/ChrisBkt) - Alexa language configuration

• [@uptimeZERO](https://github.com/uptimeZERO) - Frontend 'Now Playing' styling improvements

• [@FabionRabushja](https://github.com/FabionRabushja) - Frontend player card fixes

• [@Algram](https://github.com/Algram) - Frontend UI refresh work

• [@stvncode](https://github.com/stvncode) - Frontend breadcrumb navigation and component refactoring

• [@trisweb](https://github.com/trisweb) - Frontend UI improvements

**Continuing contributors:**

• [@marcelveldt](https://github.com/marcelveldt) - Core architecture improvements and various enhancements

• [@maximmaxim345](https://github.com/maximmaxim345) - Player management fixes and web player improvements

• [@OzGav](https://github.com/OzGav) - Multiple new providers and extensive bug fixes

• [@MarvinSchenkel](https://github.com/MarvinSchenkel) - Smart Fades implementation and pipeline improvements

• [@fmunkes](https://github.com/fmunkes) - Audiobookshelf and podcast improvements

• [@robsonke](https://github.com/robsonke) - SoundCloud enhancements and UI improvements

• [@Cyanogenbot](https://github.com/Cyanogenbot) - Bluesound multi-zone support

• [@music-assistant-machine](https://github.com/music-assistant-machine) - Automated frontend updates

• [@dependabot[bot]](https://github.com/dependabot[bot]) - Automated dependency management

A huge thank you to all our contributors for their dedication, creativity, and hard work! Your contributions make Music Assistant better for everyone. 💝

---

**Full Changelog**: https://github.com/music-assistant/server/compare/2.6.0b21...2.7.0b0

We're excited for you to try these new features and improvements! 
Remember to backup your data before updating and report any issues you encounter. Happy listening! 🎵


