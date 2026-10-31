# Signing Instructions — `v1.1.4-full-corpus-pdf`

Maintainer-only steps. They use the private key `8C8C B0D4 8C7F 60DA`.

## Step 1 — verify, sign, open PR
`PROMETHEUS_OPS_NETWORK\v1.1.4_1_sign_and_pr.ps1`

1. Copies PDF + DOCX from `_PROMETHEUS_CURRENT/03_CANDIDATE_POST_v1.1.2/` to a
   staging folder outside the repo and checks both against `SHA256SUMS.txt`.
2. Creates and verifies detached armored signatures for both assets
   (`assets/*.asc`), `RELEASE_MANIFEST.md.asc` and `SHA256SUMS.txt.asc`.
3. Commits (signed), pushes `release/v1.1.4-full-corpus-pdf`, opens a PR.

Merge the PR once `verify-release` is green.

## Step 2 — tag and release
`PROMETHEUS_OPS_NETWORK\v1.1.4_2_tag_and_release.ps1`

1. Creates and pushes the signed tag `v1.1.4-full-corpus-pdf`.
2. Publishes the GitHub release with PDF, DOCX, their `.asc`, `SHA256SUMS.txt`
   and its `.asc`, **not** marked as latest.
3. Downloads the public PDF anonymously and checks its SHA256.

## Public verification (anyone)
```bash
gpg --import keys/Uwohali_Tuccio_0x8C8CB0D48C7F60DA_public.asc
gpg --verify SHA256SUMS.txt.asc SHA256SUMS.txt
sha256sum -c SHA256SUMS.txt
gpg --verify PROMETHEUS_Canonical_White_Paper_Full_Corpus.pdf.asc \
  PROMETHEUS_Canonical_White_Paper_Full_Corpus.pdf
```
