# Firmware Artifact Audit Registry

System of record for third-party artifacts reused by the Platform Firmware Guild.

- `register.json` - machine-readable register of artifacts and verdicts
- `policy/third_party_reuse_policy.md` - reuse policy, license classes and required actions
- `artifacts/` - artifact bundles exactly as received from suppliers
- `vendor-mirrors/` - copies of public source archives retained for provenance checks

Each registry entry must name the direct source that hosts the artifact bytes and the
fingerprint file used to confirm the match. Verdicts are derived from the license that
the confirmed source declares for itself.
