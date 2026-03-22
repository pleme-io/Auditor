# Auditor (pleme-io fork)

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
