# Changelog

All notable changes to Shosho will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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
