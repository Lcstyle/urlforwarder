# URL Forwarder (Fork)

Personal fork of [daverix/urlforwarder](https://github.com/daverix/urlforwarder) with the following additions:

## Changes from upstream

- **Regex auto-forwarding** — Incorporates [PR #15](https://github.com/daverix/urlforwarder/pull/15) (regex matching + automatic URL forwarding without prompts)
- **Single share target** — Merged auto-forward logic into the main share activity so only one "URL Forwarder" option appears when sharing
- **Filter priority** — Added a priority field to filters so higher-priority filters (e.g. YouTube) run before catch-all defaults
- **ABI-split APKs** — Release builds are split by ABI (arm64-v8a, armeabi-v7a, x86_64, universal) for smaller downloads
- **GitHub Actions CI** — Automated release builds on tag push

## Downloads

Grab the latest APK from the [Releases](https://github.com/Lcstyle/urlforwarder/releases) page. Pick the APK matching your device architecture (most modern phones use `arm64-v8a`).

## Building

```
git clone https://github.com/Lcstyle/urlforwarder.git
cd urlforwarder
./gradlew assembleDebug
```

## License

Same as upstream — GPLv3.
