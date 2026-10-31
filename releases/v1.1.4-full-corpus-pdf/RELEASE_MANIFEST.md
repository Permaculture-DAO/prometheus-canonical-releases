# Release Manifest — `v1.1.4-full-corpus-pdf`

## Controlling artefacts (attached to the GitHub release)

| Asset | Bytes | SHA256 |
|---|---:|---|
| `PROMETHEUS_Canonical_White_Paper_Full_Corpus.pdf` | 9992381 | `1b50af6e7816b1264e532a13deddaeae59ef68c78b75e69c6ef11ee9ea9a98c9` |
| `PROMETHEUS_Canonical_White_Paper_Full_Corpus.docx` | 4232492 | `6f0140a9821e2546cf70665409845c7e77ccc9bd6a89a824bfb77f8319e362f8` |

- Document title (internal): `h•eart•h Prometheus - MIT Audit Integrated Canon`
- Length: 1,682 pages; ~273,500 words; 34,265 text paragraphs.
- PDF rendered from the DOCX with Microsoft Word 2019, 2026-10-31 07:02 +01:00.
- DOCX core properties: revision 388, modified 2026-06-21T11:06:00Z.

## Provenance

Maintainer workspace path:
`_PROMETHEUS_CURRENT/03_CANDIDATE_POST_v1.1.2/`

## Relation to `v1.1.2-genesis`

Base: `releases/v1.1.2-genesis/canonical/h-earth-prometheus-white-paper.docx`
(SHA256 `29f91e6d6a31fb8bd9754a7ef32ea8b7f168bf64fa7097cf9b6ee951ab9fca04`, revision 387).

A paragraph-level text comparison (34,265 vs 34,265 paragraphs) finds exactly
**one** changed paragraph, an editorial correction in a reference:

```diff
- https://github.com/Uwohali/hearthprometheuswhitepaper (github.com in Bing)
+ https://github.com/Uwohali/hearthprometheuswhitepaper
```

No other textual difference. Page count differs by one (1,681 → 1,682) due to
re-pagination. The prose content is therefore `v1.1.2-genesis` plus one editorial fix.

## Signer

Fingerprint `D20D FF6C BE33 1B3A 4109 DF84 8C8C B0D4 8C7F 60DA`
(`keys/Uwohali_Tuccio_0x8C8CB0D48C7F60DA_public.asc`).
