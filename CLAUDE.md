# Auditor (pleme-io fork)

> **★★★ CSE / Knowable Construction.** This repo operates under **Constructive Substrate Engineering** — canonical specification at [`pleme-io/theory/CONSTRUCTIVE-SUBSTRATE-ENGINEERING.md`](https://github.com/pleme-io/theory/blob/main/CONSTRUCTIVE-SUBSTRATE-ENGINEERING.md). The Compounding Directive (operational rules: solve once, load-bearing fixes only, idiom-first, models stay current, direction beats velocity) is in the org-level pleme-io/CLAUDE.md ★★★ section. Read both before non-trivial changes.


GrapheneOS hardware-based attestation and intrusion detection app.
Uses Titan M2 secure element for device integrity verification.

## Build

```bash
nix develop                      # enter Android dev shell
./gradlew assembleRelease        # build release APK
```

## Upstream

Forked from [GrapheneOS/Auditor](https://github.com/GrapheneOS/Auditor).
MIT license. Sync: `git fetch upstream && git merge upstream/main`.

## Integration with andro

- `andro-gos` crate implements `AttestationVerifier` trait
- `andro gos_status` MCP tool checks attestation state
- Future: Rust attestation client for tameshi integration
