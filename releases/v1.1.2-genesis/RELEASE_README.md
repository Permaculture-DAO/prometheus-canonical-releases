# Canonical Release — v1.1.2-genesis (2026-06-21)

Signed, frozen canonical release of the h•eart•h Prometheus v1.1 Genesis
Institutional Canonical Line. Source: `Permaculture-DAO/prometheus-canon`
(git tag `v1.1.2-genesis`, signed).

## Authorized key
`8C8CB0D48C7F60DA` — fingerprint `D20DFF6CBE331B3A4109DF848C8CB0D48C7F60DA`
(Uwohali Tuccio). Public key: `https://github.com/Uwohali.gpg`.

## Contents
- `canonical/` — White Paper of record (DOCX source of truth + MD derivation) and
  the adopted amendments A-001 (HSI / human-state weight=0) and A-002 (consolidated
  Legal Semantic Firewall).
- `constitutional/` — CAL-1.0 rider license, Syntropic Sovereignty Header, Manifesto.
- `RELEASE_NOTES.md`, `RELEASE_MANIFEST.md`, `RELEASE_SIGNING_READINESS.md`, `CHANGELOG.md`.
- `bundles/` — detached `.asc` signatures for the Holochain runtime bundles
  (`hearth_prometheus.happ`, `hearth_prometheus_web.webhapp`, `hearth.dna`). The
  bundles themselves are distributed via the GitHub Release (built artifacts),
  with these signatures and the SHA256 in `RELEASE_MANIFEST.md`.
- `SHA256_SUMS.txt` — checksums of every file in this release directory.
- A detached `.asc` accompanies every signed file.

## Verify
```bash
# import the public key (once)
curl -sL https://github.com/Uwohali.gpg | gpg --import
# verify any file
gpg --verify RELEASE_NOTES.md.asc RELEASE_NOTES.md
gpg --verify canonical/h-earth-prometheus-white-paper.docx.asc canonical/h-earth-prometheus-white-paper.docx
# verify all checksums
sha256sum -c SHA256_SUMS.txt
# verify the git tag (in a clone of prometheus-canon)
git verify-tag v1.1.2-genesis
```

## Custody disclosure
This release is **substantially single-source**: signed by a **single authority**,
not yet shaped by more than one authoring process nor ratified by multiple active
stewards. The signature attests **authenticity and integrity**, not multi-steward
constitutional ratification. Amendments A-001/A-002 are adopted as versioned
clauses; their incorporation into the WP prose body is deferred to v1.1.3.

This release creates no PRU value, RAP class, admissibility, or any
land/cash-flow/governance/investor right. Evidence before value; the lowest
unresolved gate controls the permitted claim.
