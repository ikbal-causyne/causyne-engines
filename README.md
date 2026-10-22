# Causyne Engines

Native headless engine binaries for Causyne Agent. Under active development.

## Available engines

| Engine | Binary | Version | Platforms |
|---|---|---|---|
| Film | `causyne-engine-film` | 0.1.0 | macOS arm64 |

Causyne Agent downloads an engine release on request and verifies its SHA-256
before installing it under `~/.causyne/engines/`.

## Manual download

Download the binary for your platform from the latest release, make it
executable, and run:

```sh
chmod +x causyne-engine-film-darwin-arm64
./causyne-engine-film-darwin-arm64 --version
./causyne-engine-film-darwin-arm64 help
```

The macOS arm64 binary is ad-hoc signed, not notarized. On first launch, use
Finder's Open command or allow it in System Settings if macOS blocks it.

## Manifest

`engines.json` is the release manifest consumed by the Causyne Agent installer.
It is published with every release.
