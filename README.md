# Gamelauncher-model-rife

Download-only distribution scaffold for the GameLauncher **rife** model.

Repository: https://github.com/nekobyran/Gamelauncher-model-rife

Upstream: https://github.com/hzwer/ECCV2022-RIFE

## Rules

- This repository contains no games and no game data.
- Artifacts are published per client platform and ABI under `artifacts/<platform>/<abi>/`.
- A release `runtime-component-manifest.json` must validate against `manifest.schema.json`.
- `manifest.example.json` is documentation only and must never be published.
- Every artifact must have its real byte length and lowercase SHA-256 in the release manifest and `checksums.sha256`.
- The GameLauncher project repository is the default source. Upstream official sources are optional and may have compatibility differences.
- No binary payload is committed by this scaffold. Publish release artifacts only after license and provenance review.

## Supported slots

| Platform | ABI slots |
| --- | --- |
| android | arm64-v8a, armeabi-v7a, x86_64, x86 |
| windows | x64, arm64 |
| linux | x64, arm64 |
| macos | x64, arm64 |
| ios | arm64, simulator-arm64, simulator-x64 |

## Licensing

Scaffold metadata and documentation use `MIT`. Distributed RIFE payloads retain their upstream `MIT` terms. See `THIRD_PARTY_NOTICES.md`.
