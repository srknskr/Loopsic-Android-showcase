# Loopsic for Android

> A rhythm and loop practice application for discovering, creating, organizing, and playing musical loops.

**Platform:** Android  
**Application version:** 4.2.4 (version code 141)  
**Source code:** Private

> Google Play link will be added.

## About

Loopsic is a native Android music application centered on loop playback, BPM practice, playlist organization, and custom loop creation. Its private implementation combines a Java Android application with a local data layer, playback services, an equalizer module, premium content, notifications, and media integrations.

## Screenshots

> Screenshots will be added here.

| Home | Loop player | Playlist and BPM |
|---|---|---|
| Coming soon | Coming soon | Coming soon |

## Architecture

The application is organized around Android Activities and Views, feature-specific UI packages, data models, adapters, services, receivers, and local persistence.

~~~mermaid
flowchart TB
    UI[Activities and Android Views] --> FEATURES[Home, playlists, custom loops, BPM, shop, user]
    FEATURES --> DATA[Models, adapters, listeners, helpers]
    DATA --> ROOM[Room local database]
    FEATURES --> PLAYER[Playback and media services]
    PLAYER --> MEDIA[Android media APIs and ExoPlayer]
    FEATURES --> EQ[Equalizer module]
    FEATURES --> NOTIFY[Firebase messaging and notification receiver]
    FEATURES --> PREMIUM[Premium content and purchases]
    PREMIUM --> BILLING[Google Play Billing]
~~~

## Product Experience

- Browse and play musical loops
- Create and manage custom loops
- Organize loops in playlists
- Save BPM sessions and revisit BPM details
- Repeat mode and playback controls
- Equalizer support
- Premium variation and genre packs
- Shop and user areas
- Firebase notifications
- App rating and review flow
- Background playback and service-based media handling

## Technology Stack

| Area | Technologies found in the private project |
|---|---|
| Language | Java |
| UI | Android Views, Material Components, ConstraintLayout, View Binding |
| Architecture | Feature-oriented Android structure with lifecycle-aware data and UI components |
| Navigation | Navigation Fragment and Navigation UI |
| Persistence | Room |
| Media | AndroidX Media and ExoPlayer |
| Audio | Dedicated equalizer module |
| Services | Firebase Analytics and Firebase Cloud Messaging |
| Monetization | Google Play Billing and rewarded-ad flow |
| Images | Glide |
| Background work | AndroidX WorkManager |
| Testing | JUnit, AndroidX Test, Espresso |
| Build baseline | minSdk 26, target/compile SDK 36, JVM target 17 |

## High-Level Project Map

- Home and loop discovery
- Playlist list and playlist detail
- Custom loop creation and collection
- Saved BPM and BPM detail
- Shop and user screens
- Data, models, adapters, listeners, helpers, receivers, and services
- Playback and notification services
- Equalizer and local Room storage

## Privacy and Source Code

This repository is a public product showcase. It contains documentation and presentation material only.

The application source code, private audio assets, service configuration, signing material, and release secrets remain in the private project.

## Credits

Developed by Serkan Şeker.
