# Cuff Link

Distribution repo for a personal Android TV app.

- **Latest APK:** https://github.com/xxxtastytestxxx-svg/cuff-link/releases/latest/download/cuff-link.apk
- **`rules.json`:** read by the app every few hours. It holds site URL fixes, extra ad hosts,
  and the current version (`update.versionCode`). When that number is higher than the
  installed app's, the app's Settings screen offers to download and install `apkUrl`.

## Releasing a new version

1. Bump `versionCode` / `versionName` in the app and build the release APK.
2. Publish a GitHub release with the APK attached as `cuff-link.apk`.
3. Raise `update.versionCode` / `versionName` in `rules.json` to match.
