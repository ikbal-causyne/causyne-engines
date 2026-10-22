# Causyne Engines

Native headless engine binaries for Causyne Agent. Under active development.

## Available engines

| Engine | Binary | Version | Platforms |
|---|---|---|---|
| Film | `causyne-engine-film` | 0.1.1 | macOS arm64, Linux x64, Windows x64 |
| Photo | `causyne-engine-photo` | 0.8.2 | macOS arm64 |
| Sound | `causyne-engine-sound` | 0.6.1 | macOS arm64 |
| CAD | `causyne-engine-cad` | 0.6.2 | macOS arm64 |
| Deck | `causyne-engine-deck` | 0.1.0 | macOS arm64, Linux x64, Windows x64 |
| Design | `causyne-engine-design` | 0.7.1 | macOS arm64 |
| Word | `causyne-engine-word` | 0.6.1 | macOS arm64 |
| Grid | `causyne-engine-grid` | 0.6.1 | macOS arm64 |
| Light | `causyne-engine-light` | 0.7.1 | macOS arm64 |
| PDF | `causyne-engine-pdf` | 0.7.1 | macOS arm64 |
| Effect | `causyne-engine-effect` | 0.9.2 | macOS arm64 |

Causyne Agent downloads an engine release on request and verifies its SHA-256
before installing it under `~/.causyne/engines/`.

## Manual download

Download the binary for your engine and platform from its release, make it
executable, and run:

```sh
chmod +x causyne-engine-deck-darwin-arm64
./causyne-engine-deck-darwin-arm64 --version
./causyne-engine-deck-darwin-arm64 help
```

Use `causyne-engine-deck-linux-x64` on Linux x64 and
`causyne-engine-deck-win32-x64.exe` on Windows x64.

The macOS arm64 binary is ad-hoc signed, not notarized. On first launch, use
Finder's Open command or allow it in System Settings if macOS blocks it. The
Windows binary is unsigned.

## Notices

Each engine bundles third-party Rust crates. Each release includes its own
`THIRD_PARTY_NOTICES.md`, `THIRD_PARTY_LICENSES.md` and attribution files.

## Manifest

`engines.json` is the release manifest consumed by the Causyne Agent installer.
It is published with every release.
