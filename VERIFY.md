# Verify a Release

## 1. Import the public key

```bash
gpg --import keys/Uwohali_Tuccio_0x8C8CB0D48C7F60DA_public.asc
gpg --fingerprint 8C8CB0D48C7F60DA
```

Expected fingerprint:

```text
D20D FF6C BE33 1B3A 4109 DF84 8C8C B0D4 8C7F 60DA
```

## 2. Verify the release files

```bash
cd releases/v1.1.2-genesis
sha256sum -c SHA256_SUMS.txt
gpg --verify RELEASE_MANIFEST.md.asc RELEASE_MANIFEST.md
gpg --verify canonical/h-earth-prometheus-white-paper.docx.asc \
  canonical/h-earth-prometheus-white-paper.docx
```

Every signed file has a sibling `.asc` file.

## 3. Verify runtime release assets

Download the runtime assets attached to the GitHub release, then run:

```bash
gpg --verify hearth_prometheus.happ.asc hearth_prometheus.happ
gpg --verify hearth_prometheus_web.webhapp.asc hearth_prometheus_web.webhapp
gpg --verify hearth.dna.asc hearth.dna
```

The expected bundle hashes are recorded in `RELEASE_MANIFEST.md`.

## 4. Verify the source tag

```bash
git clone https://github.com/Permaculture-DAO/prometheus-canon.git
cd prometheus-canon
git verify-tag v1.1.2-genesis
```
