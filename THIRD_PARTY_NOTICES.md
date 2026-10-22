# Third-party notices

The Causyne Film Engine binary is built with open-source Rust crates. The
external crates linked directly by the engine binary are:

| Package | Version | License |
|---|---|---|
| `image` | 0.25.10 | MIT OR Apache-2.0 |
| `serde_json` | 1.0.151 | MIT OR Apache-2.0 |

The binary also links transitive dependencies of these crates and of the
engine source. Their license texts and copyright notices are available from
their published crates.io packages and from the dependency metadata of the
build. Packages that ship a NOTICE file carry that notice with their package.

The full MIT license for the engine source is in `LICENSE`.
