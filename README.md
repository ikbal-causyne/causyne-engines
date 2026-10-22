# Causyne Engines

Native headless engine binaries for Causyne Agent. Under active development.

## Available engines

| Engine | Binary | Version | Platforms |
|---|---|---|---|
| Film | `causyne-engine-film` | 0.1.1 | macOS arm64, Linux x64, Windows x64 |
| Photo | `causyne-engine-photo` | 0.8.2 | macOS arm64, Linux x64, Windows x64 |
| Sound | `causyne-engine-sound` | 0.6.1 | macOS arm64, Linux x64, Windows x64 |
| CAD | `causyne-engine-cad` | 0.6.2 | macOS arm64, Linux x64, Windows x64 |

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

Use `causyne-engine-film-linux-x64` on Linux x64 and
`causyne-engine-film-win32-x64.exe` on Windows x64.

The macOS arm64 binary is ad-hoc signed, not notarized. On first launch, use
Finder's Open command or allow it in System Settings if macOS blocks it. The
Windows binary is unsigned.

## Notices

The engine bundles third-party Rust crates. The dependency list and elected
licenses are in [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md); the full
license texts and copyright notices are in
[`THIRD_PARTY_LICENSES.md`](THIRD_PARTY_LICENSES.md).

## Manifest

`engines.json` is the release manifest consumed by the Causyne Agent installer.
It is published with every release.
