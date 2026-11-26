# AetherLink Mobile fork changes

This public repository is a modified fork of https://github.com/hiddify/hiddify-app.
It remains under the Hiddify Extended GPL v3 terms in `LICENSE.md`, including all
additional conditions.

## Current fork changes

- Renamed the Android application label to AetherLink Mobile.
- Replaced the upstream-branded README introduction with fork attribution, license,
  non-commercial personal-use and distribution notices.
- Added a GitHub Actions workflow that builds and attaches ARM64 and universal Android
  APKs to releases created from `aetherlink-v*` tags.
- Switched the public `hiddify-core` submodule URL to HTTPS so Actions can check out
  source without a personal SSH key.

## Integration status

The Hiddify VPN and per-app routing implementation is retained. AetherLink's transport
protocol is not yet wired into Hiddify's sing-box core; existing profile/protocol
functionality remains until a tested AetherLink outbound is implemented. Builds from
this revision must not be described as AetherLink-protocol compatible.
