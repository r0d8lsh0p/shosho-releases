# Changelog

All notable changes to Shosho will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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
