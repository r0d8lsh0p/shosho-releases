# Changelog

All notable changes to Shosho will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-08-31

### Added

- More live streams! Integrated live streams from the Livelier.live bridge so you will find more new creators, gamers, artists and live music
- Improved curation of lives streams in the browse screen
- Separated Live and Replay browse rails

### Changed

- Improved deep links now read from relay-hints
- Improved sharing now shares with relay-hints
- Improved stream chat reads and posts from live-stream’s chat relays
- NSFW content is filtered from the browse screen
- NSFW creators can tag their content "NSFW" on the Shows and Clips screens

### Fixed

- Improvements to revalidate stale cached profiles

## [1.0.0] - TBD

### Added

- Full app redesign! Shosho is putting content first. New home screen, carousel, bottom tab bar, and a one-tap creator menu to go live, add a show, clip, or product
- Notifications! See your mentions, reactions, reposts, and zaps in one feed, and reply to any of them without leaving the app. Plus all the latest lives and clips from people you follow
- Search! Search and jump to your favourite Creators, Lives, Clips, and Products on the Shosho Relay, or set your own search relays in settings
- Instant live stream clipping! Create a clip from any live or replay and publish it without missing a live moment
- Localised in 9 languages: English, French, German, Spanish, Portuguese, Chinese, Korean, Japanese, and Thai

### Changed

- Shosho is now a Live Streaming Marketplace — refreshed wording across the app
- Clips you're tagged in now appear on your profile alongside your own clips
- Smarter video display — landscape videos fit, clips fill the screen
- Edge-to-edge display on older Android devices too, not just new ones
- Featured creators now ranked by their most recent streams and clips
- Improved threading and layout in chat panel
- Improved support for clip replies and threaded replies
- Performance improvements, faster profile loading, and less network traffic

### Fixed

- Improved Hell Thread Protection with "Hide Indirect Mentions" in settings
- Live badge in the player now tracks the stream's real status on the network
- Screen stays awake during playback as it should
- Picture-in-Picture stability improvements on Android and iOS
- Many small UI and stability improvements

## [0.16.0] - 2026-05-26

### Added

- Shosho Shopping Cart! Add products to cart and check out without leaving the stream
- Shosho Seller Hub! A fully featured backend for selling your products on Shosho – create a Shop, list products, set stock locations and shipping, manage inventory, offer promotions, receive and fulfil orders, and more
- Shosho Help Center! Everything you need to know to stream on Shosho and sell on Shosho Shopping Cart

### Changed

- Short video clips including Divine Clips are now available in the Shosho feed
- More expansive featured content on the Browse screen from the Shosho WOT Relay
- Use your Nostr identity to log in and manage your Shop
- Faster loading of Clips and Streams on browse
- Faster opening of lives when you land from a deep link

### Fixed

- Picture-in-Picture return-to-fullscreen now opens the correct video in the carousel
- Many small UI and stability improvements

## [0.15.2] - 2026-04-09

### Fixed

- Improved keyboard handling on Android
- Fixed status bar colour issues on Android
- Fixed screen rotation on live stream carousel

## [0.15.1] - 2026-04-07

### Fixed

- Keyboard hiding live stream chat input

## [0.15.0] - 2026-04-07

### Added

- Shows! Set up custom show info before you go live, and connect your show to OBS or any encoder
- TikTok-style vertical video carousel! Swipe through lives, clips, and replays in a full-screen feed
- Quick Add for Shows, Clips, and Products – publish video clips and add products directly from your profile

### Changed

- Refreshed UI across clips and products
- More featured streamers, clippers, and sellers in the browse screen

### Fixed

- Fixed "Live Now" showing on profiles after streams had ended
- Fixed some streams not playing back correctly
- Fixed some product descriptions displaying incorrectly in Shop

## [0.14.0] - 2026-03-12

### Added

- The launch of Shosho Shop! Link to your products directly from your live streams and clips. There is nothing to set up – All your Nostr products will automatically appear in your Shosho Shop, and your friends and followers can click through to purchase from your page on Plebeian Market
- Follow streamers from the app, and get push notifications when they go live
- Subscription to each Host's relays so you don't miss chat messages
- Auto-reconnection on relay disconnects for long-lived streams

### Changed

- Added Shop tab to all Shosho profiles
- Added Shop to Browse Screen and made sideways scrolling
- Added In-Live Shop button to all Lives and Clips
- Improved performance and speed on Browse Screen
- Removed Nostr.Band from default relays
- Added mute button to iOS broadcast
- General performance improvements

### Fixed

- Fixed bug that muted audio on iOS when camera changed on broadcast
- Fixed bug where mute button did not work on Android on broadcast
- Fixed browse screen only showing a handful of featured streamers

## [0.13.0] - 2026-02-27

### Added

- Download your replays as MP4s by pressing Download from stream card menu
- NIP-05 verification for Nostr profiles

### Changed

- Improved streaming performance
- Migrated RTMP publisher to Expo Modules API and New Architecture
- Improved presentation of bech32 IDs in chat

### Fixed

- Improved streaming connections on lower bandwidth
- Fixed certain streaming crashes on old devices
- Fixed streaming with iOS devices to Zap.Stream server 
- Fixed a bug where camera preferences were not being respected

## [0.12.0] - 2026-02-12

### Added

- Clips! Watch video clips from your favourite creators and reply to Clips in the player. Compatible with Divine, Plebs, Olas and other great Nostr apps
- Custom Emojis! Use your emojito.meme emojis in your chat by pressing ":"
- Hell Thread Protection. You can now turn off indirect mentions in app settings to prevent spam
- Improved playback view for landscape videos, similar to Twitch playback
- Share Profiles with QR codes
- Improved profiles for your favourite streamers

### Changed

- Browse streams screen updated to include clips from featured creators

### Fixed

- Minor bug fixes

## [0.11.1] - 2026-01-30

### Added

- New streaming server! Shosho Server is now our default server with recording and video on demand playback of your live streams
- Room Presence! Shosho will publish when you join a live and show you who joined when you're live
- Threaded Chats! Reply to messages and see threaded replies in busy chats
- Login with Nostr Connect including on iOS! (works with Primal Remote Login)
- Add new servers to your Shosho app by clicking links or scanning QR codes
- Share servers between devices
- Manage your relays in the app
- Update your stream image with a simple uploader and save to nostr.build
- Toasts on all UI actions (copy, mute, etc)
- and Dark Mode!

### Changed

- Faster chat messaging
- Wider delete publishing
- Added QR codes for lightning payments
- Upgraded to Expo 54

### Fixed

- Fixed old Zap Sream server details, now updated to the new zap stream API URL (use this or the new Shosho Server if you prefer)
- Fixed bug where mute lists would not persist on chats
- Fixed ToS URL for custom Nostr servers
- Fixed some deep links not deep linking
- Fixed many other small bugs and improved UI
- Smoother PiP transitions
- Updated all Testflight links to full Apple Store release

## [0.10.1] - 2025-11-11

### Fixed

- Fixed: Android in-app Picture-in-Picture buttons were not pressable on some handsets
- Fixed: Android regression on broadcast screen so that preview wasn't always full height on some handsets  
- iOS required a "purpose string" for use of image permissions in edit profile

## [0.10.0] - 2025-11-10

### Added

- Picture in Picture mode
- Lock screen playback controls
- Camera screen to set your camera preferences
- Remember camera facing preferences between sessions
- Edit profile screen to build your streamer profile
- Streamers can get custom URLs like shosho.live/nogood
- Promote your live before you start, press "share" to send your followers to your custom URL
- Nostr.build image uploads for profiles
- Prompt new Nostr users for a username before chat
- Pull to refresh on profiles, browse streams, server and camera settings
- Improved handling for permissions denied on splash screen
- Responsive controls condense on landscape mode
- Push notifications ready

### Changed

- Improved handling of different cameras (especially on iPhone)
- Improved handling of stream errors
- Improved monitoring for streaming server disconnections
- Automated testing

### Fixed

- Fall back to stream Thumbnail if Image is not available
- Filter out 30311 events that are not .m3u8 live streams (e.g. Corny Chat)
- More forgiving on some text fields in user-friendly ways
- Minor bugs with caches, navigation

### Note for iOS

- We still have a bug that prevents some iOS handsets from going live to Zap.Stream server
- Android works on any server
- iOS works on any other server than Zap.Stream
- We are working on this!

## [0.9.0] - 2025-10-08

### Added

- Improved browse screen now with more lives and replays, less spam
- Responsive for browsing on tablets and larger devices
- Share your live stream and profile for followers to join you on shosho.live
- Links to shosho.live deep link into the app on iOS and Android
- More options on chat messages, profiles and lives including: reply, copy text, copy note ID, delete, hide, mute, report
- Delete your old streams function works with both self-hosted and Zap Stream APIs (will publish a Kind 5 for self-hosted streams or connect to a Nostr Streaming Server API for hosted streams)
- Global Shosho mute list for hiding spam and test users
- Connecting and Disconnecting states on broadcast screen
- Display custom emojis in chat

### Changed

- Improved broadcast screen and going-live UX
- Improved browse screen scroll
- Moved browse menu into a menu drawer (click your profile to see your new menu)
- Navigate to streamer profiles from browse screen
- Faster connections to Nostr stream chat
- Refactored go live process for consistency and handling of errors and failures
- Refactored Expo, Yarn, contexts and other plumbing to run app and web on same code

### Fixed

- Fixed integration with the new Zap Stream Core backend. Back to "one click to go live"
- Bugs with Auth context, duplicate Amber signing requests, and adding new servers
- Server settings tells you which server you're on
- Lots more attention paid to iOS-specific bugs
- Profile paths use npub not hexpub
- Readme links to Play Store

## [0.8.0] - 2025-01-08

### Added

- Set up and stream to any RTMP server not just Zap.Stream
- Your live stream appears on Nostr no matter which server you choose
- Added server screen
- Ability to configure multiple servers
- Select from your choice of server
- Settings for Generic and Nostr stream providers
- Set custom stream metadata for each server

### Changed

- Stream Confirmation Buttomsheet now directs to Servers
- Nostr stream providers rely upon server to publish your live event
- Generic stream providers publish your live event from shosho

### Fixed

- Bugged error states on connection failures for iOS
- UX improvements for smaller phones, landscape mode, Nostr Stream Provider setup and onboarding

### Notes with Amber

If you use Amber Signer, please set to automatically approve 30311 events from Shosho. If instead you leave Amber with manual approval on 30311 events Shosho may leave your live stream mid-stream to request a signature, which is a little annoying when you are live!

## [0.7.0] - 2025-07-14

### Added

- More speed and stability!
- Improved error handling and messaging when failing to connect

### Changed

- Improved loading on splash screen so broadcast is more responsive
- Improved focus handling so all screens respond immediately instead of being held up by last screen's subscriptions
- Tidied up safe view areas, headers, and animations throughout the app
- Refactored browse streams screen and streams view on profile screen for speed and stability with context, cache, store, and improved pagination
- Refactored chat panel for speed and stability with context, cache, store, and process note contents prior to rendering them for less jumping around
- Refactored contexts to improve performance and remove unnecessary reloads of chat panel
- Improved profile loading batching to avoid relay timeouts
- Better error messaging when streaming server cannot be connected
- More improvements for small and old phones
- Improved routes for deeplinks from shosho.live website (coming soon)

### Fixed

- Replays and offline views no longer display unrelated emotes and zaps
- Video player now respects safe area view
- Bug where browse page wouldn't reload
- But where swipeable UI would stop working
- Many other bugs!

### Removed

- Mute button wouldn't unmute on iOS

## [0.6.4] - 2025-06-27

### Added

- Camera device detection for Android handsets

### Changed

- Use detected cameras and make no guesses
- Gracefully fallback to common defaults if absent
- Try connections twice and show modal if fails

### Fixed

- Avoid camera freeze or black out on old handsets

## [0.6.3] - 2025-06-24

### Fixed

- Fixed Android release signing configuration to use production keystore

## [0.6.2] - 2025-06-24

### Fixed

- Reverted Android configuration to maintain compatibility with existing installations

## [0.6.1] - 2025-06-24

**NOTE:** Users who experienced blocking and freezing on streams may try this updated version, hopefully we have fixed it temporarily by reducing the bandwidth requirements. Please give your feedback, if this has worked, we will make it configurable and adaptive to network conditions in future versions.

### Added

- shosho now on both Android and iOS
- released to TestFlight on iOS
- handling for more bech32 kinds

### Changed

- RTMP streaming library updated
- RTMP settings update to remove blocking and freezing
- Default relays changed to WOT, reduced spam for new users
- More elegant permission requests
- Expo version updated
- Minor UI improvements

### Fixed

- Text layout on certain profile bios
- Text layout on certain chat messages
- Keyboard handling in certain situations
- Navigation from profile to profile
- Lazy loading of prior streams in profile page
- More minor bugs crushed

## [0.5.1] - 2025-06-12

### Fixed

- Bug with server config when switching users

## [0.5.0] - 2025-06-11

### Added

- Fun floating emojis!
- Double-tap video-player to emote
- Display emotes in stream chat
- Landscape mode on player screen
- Wake lock on player screen
- Swipe to hide UI on broadcast and player screens

### Changed

- Improved layout for smaller devices
- Refactoring for upcoming iOS release

### Fixed

- Set Zap.Stream meta information correctly
- Calculate Zap.Stream cost and time remaining correctly
- Many other small bugs

## [0.4.1] - 2025-06-05

### Fixed

- Fixed changelog processing in GitHub Actions workflow

## [0.4.0] - 2025-06-05

### Added

- Streamlined Go Live for first time users
- No Zapstream balance required, start with 0 sats!
- Browse lives
- Featured lives and streamers
- Watch lives and replays
- Full screen mode with landscape and scrubbing
- Better loading, caches, skeletons, and lazy loads

### Changed

- A big refactor of all Nostr network touchpoints

### Fixed

- Countless small bugs

## [0.3.1] - 2025-05-28

### Added
- Better start stream workflow in case of users not ready to stream

### Changed
- Default tab is "all" messages

### Fixed
- Profile pictures display in chat panel
- Custom URL in config screen

## [0.3.0] - 2025-05-27

### Added
- Configure zapstream from inside shosho
- Tag users by pressing them in chat
- Handling for more chat message inclusions, npubs, nprofiles, URLs, etc, in chat and on profile page

### Improved
- Use zapstream free tier by default
- Profile and message loading and caching

### Fixed
- Corrected fonts and colours
- Amber signer auth timeout
- Lengthen zapstream API call caching
- Zaps show correct amounts
- Use users relays
- Try again to get on zapstore!

## [0.2.3] - 2025-05-19

### Fixed

- Fix for ZapStore process
- Fix for Android versionCode

## [0.2.2] - 2025-05-19

### Fixed

- Fix for ZapStore process
- Updated target API level to 34 (Android 14) for Google Play Store compliance

## [0.2.1] - 2025-05-19

### Fixed

- Fix for ZapStore process

## [0.2.0] - 2025-05-19

### Added

- Stay awake on broadcast screen
- Privacy Policy in releases repo
- Now available on ZapStore

### Improved

- Broadcast UI
- Colour scheme
- Consistent fonts
- Test coverage

### Fixed

- Correct build flag for Play Store

## [0.1.5] - 2025-05-15

### Changed

- Updated GitHub Actions workflow
- Added GitHub Release creation in shosho-releases repository
- Added README.md to release artifacts

## [0.1.4] - 2025-05-15

### Fixed

- Fixed permissions for Github Actions

## [0.1.3] - 2025-05-15

### Fixed

- Fixed GitHub Actions release process

## [0.1.2] - 2025-05-15

### Fixed

- Updated .gitignore to allow tracking of native files
- Committed missing Amber native modules to support custom Android functionality

## [0.1.1] - 2025-05-15

### Fixed

- GitHub Actions workflow updated

## [0.1.0] - 2025-05-15

This is the initial release of Shosho, a Nostr-native RTMP Live Streaming App.

### Live Streaming

- RTMP streaming to go live to your friends and followers
- Camera controls for switching between front and back cameras
- Stream status indicators and connection management
- Zap.Stream integration

### Nostr Integration

- Nostr integration with support for multiple Nostr accounts
- Sign in with Amber or Nsec
- Support for user relays
- Support for kinds 1, 1311, 9735, 30311, etc

### Interactive Features

- Live chat with your friends and followers
- Receive zaps in your stream
- Profile views with prior streams
- Watch stream recording replays with chats from previous streams

### UI/UX

- Nice broadcasting and chat screen
- Responsive design for different device sizes

## Known Issues

- None reported yet but this is the first release, so please expect bugs!
- Please help by reporting bugs as Github Issues or message Rod on Nostr at npub1r0d8u8mnj6769500nypnm28a9hpk9qg8jr0ehe30tygr3wuhcnvs4rfsft

## Coming Soon

- Chat actions for easy replies and reactions when you're live
- Emotes and zaps on your stream
- Enhanced stream browser and playback
- iOS version
- More

[1.1.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v1.1.0
[1.0.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v1.0.0
[0.16.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.16.0
[0.15.2]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.15.2
[0.15.1]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.15.1
[0.15.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.15.0
[0.14.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.14.0
[0.13.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.13.0
[0.12.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.12.0
[0.11.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.11.1
[0.10.1]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.10.1
[0.10.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.10.0
[0.9.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.9.0
[0.8.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.8.0
[0.7.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.7.0
[0.6.4]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.6.4
[0.6.3]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.6.3
[0.6.2]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.6.2
[0.6.1]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.6.1
[0.5.1]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.5.1
[0.5.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.5.0
[0.4.1]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.4.1
[0.4.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.4.0
[0.3.1]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.3.1
[0.3.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.3.0
[0.2.3]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.2.3
[0.2.2]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.2.2
[0.2.1]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.2.1
[0.2.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.2.0
[0.1.5]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.1.5
[0.1.4]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.1.4
[0.1.3]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.1.3
[0.1.2]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.1.2
[0.1.1]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.1.1
[0.1.0]: https://github.com/r0d8lsh0p/shosho-releases/releases/tag/v0.1.0
