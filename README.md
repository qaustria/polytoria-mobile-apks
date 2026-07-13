# Polytoria 2.0 Mobile APK Archive

Automated Android APK builds for [Polytoria 2.0](https://github.com/Polytoria/polytoria-game).

## Downloads

### Stable Releases
Stable APKs are built from official Polytoria releases. Each release tag (e.g. `2.0.19`) has a corresponding APK.

**[Latest Stable Release](https://github.com/qaustria/polytoria-mobile-apks/releases/latest)**

### Dev Builds
Dev APKs are built daily from the latest commits on the Polytoria main branch. These may be unstable.

**[Latest Dev Build](https://github.com/qaustria/polytoria-mobile-apks/releases/tag/dev-latest)**

## How It Works

This repository uses GitHub Actions to automatically build Android APKs from the [Polytoria source code](https://github.com/Polytoria/polytoria-game).

### Stable Builds
- Triggered manually with a specific release tag, or weekly on Monday
- Builds the exact same code as the official Polytoria release
- Creates a GitHub Release with the APK attached

### Dev Builds
- Triggered daily at 12:00 UTC or manually
- Builds from the latest `main` branch commits
- Updates the `dev-latest` pre-release tag with the newest build
- Previous dev APKs are replaced (only the latest is kept)

## Installation

1. Download the APK from [Releases](https://github.com/qaustria/polytoria-mobile-apks/releases)
2. On your Android device, enable **Install from unknown sources** in Settings > Security
3. Open the downloaded APK file to install
4. Launch Polytoria from your app drawer

## Requirements

- Android 7.0 (API 24) or higher
- ARM64 device (most modern Android phones)

## Building Manually

You can trigger a build manually from the [Actions](https://github.com/qaustria/polytoria-mobile-apks/actions) tab:

1. Go to **Actions** > **Build Stable APK** or **Build Dev APK**
2. Click **Run workflow**
3. For stable builds, optionally enter a Polytoria release tag (e.g. `2.0.19`)
4. Click the green **Run workflow** button

## Disclaimer

This is an **unofficial** automated build service. These APKs are not affiliated with or endorsed by Polytoria. For official downloads, visit [polytoria.com](https://polytoria.com).

## License

Polytoria is licensed under the [Mozilla Public License 2.0](https://github.com/Polytoria/polytoria-game/blob/main/LICENSE). The automation scripts in this repository are provided as-is.
