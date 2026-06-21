# Changelog

## [0.12.2] - 2026-06-21
### Changed
- **Requires AndroidAwnCore 0.12.2.**

## [0.12.1] - 2026-06-21
### Updated
- **Native library updated:** AndroidAwnCore updated to 0.12.1.

## [0.11.0] - 2025-02-13
### Breaking changes
- **License key validation removed:** The `LicenseManager`, `Crypto`, and `Encoder` classes have been completely removed. The `licenseKeys` parameter was removed from `AwesomeNotificationsFcm.initialize()` and `FcmDefaultsManager.saveDefault()`. Notifications are no longer watermarked with `[DEMO]` prefix on release builds.
- **Build system updated:** AGP 8.1.1 → 8.13.1, Gradle 8.10 → 8.13, compileSdk/targetSdk 34 → 36, dependencies updated (guava 33.5.0, annotation 1.9.1).

### Updated
- **Native library updated:** AndroidAwnCore updated to 0.11.0.
- **Dependencies updated:** play-services-base 18.5.0 → 18.10.0, guava 32.1.3 → 33.5.0, appcompat 1.7.1, material 1.13.0, annotation 1.9.1.

### Fixed
- **Conflicting `compileSdk 36`:** Removed duplicate `compileSdk` inside `defaultConfig` that shadowed the root-level `compileSdkVersion = 36`.
