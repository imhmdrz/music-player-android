# Music Player for Android

A local Android music player built with Kotlin, MVVM, ExoPlayer, and notification playback controls.

## Highlights

- Browse audio stored on the device.
- Play tracks with ExoPlayer.
- Control playback through a player service and media notification.
- Organize UI and playback state with MVVM, LiveData, and a repository.

**Stack:** Kotlin · Android Views · MVVM · ExoPlayer · MediaSession · Coil

## Getting started

Use Android Studio with JDK 17, Android SDK 33, and a device or emulator running Android API 29 or newer.

```bash
git clone https://github.com/imhmdrz/music-player-android.git
cd music-player-android
./gradlew :app:assembleDebug
```

Open the repository in Android Studio, let Gradle sync, and run the `app` configuration. On Windows, use `gradlew.bat` in place of `./gradlew`.

Add audio files to the test device and grant the requested media access. A physical device is useful for checking notification controls and playback behavior.

## Code map

Paths below are relative to `app/src/main/java/com/example/musicplayer/`.

| Directory | Responsibility |
| --- | --- |
| `fragments/` | Library and player screens |
| `service/` | Player service |
| `playerListener/` | Playback and seek callbacks |
| `repository/` | Song data |
| `viewModel/` | UI state and ViewModel creation |

This project uses the original `com.google.android.exoplayer` packages. A move to AndroidX Media3 would be a separate code migration.
