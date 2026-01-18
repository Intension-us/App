# Intension App Releases

This repository hosts the release artifacts for [Intension](https://github.com/Intension-us/intension-mac) macOS application.

## Contents

- `appcast.xml` - Sparkle update feed for automatic updates
- GitHub Releases - Notarized and signed `.zip` archives

## For Users

The app automatically checks for updates using the Sparkle framework. You can also manually check via **Intension → Check for Updates...** in the menu bar.

## For Developers

### Release Process

See the [Release Documentation](https://github.com/Intension-us/intension-mac/blob/main/RELEASE.md) in the main repository.

### Appcast Structure

Each release entry in `appcast.xml` contains:
- Version information (`sparkle:version` = build number, `sparkle:shortVersionString` = marketing version)
- EdDSA signature for secure verification
- Download URL pointing to GitHub Releases
- Release notes in HTML format

### Security

All releases are:
- Code signed with Apple Developer ID
- Notarized by Apple
- Signed with EdDSA for Sparkle verification

## Links

- [Main Repository](https://github.com/Intension-us/intension-mac)
- [Sparkle Framework](https://sparkle-project.org/)
