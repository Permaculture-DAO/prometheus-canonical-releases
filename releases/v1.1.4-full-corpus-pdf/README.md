# `v1.1.4-full-corpus-pdf` — signing-ready CANDIDATE package

**Status: SIGNED (not the current canonical release).** Prepared for the maintainer to review,
sign and publish. A **document-rendition** release: it distributes the full White
Paper corpus as PDF and DOCX. The current canonical prose release remains
`v1.1.2-genesis` until a separate, explicit ratification says otherwise.

| File | What |
|---|---|
| `RELEASE_MANIFEST.md` | controlling artefacts, SHA256, sizes, provenance, diff vs v1.1.2-genesis |
| `RELEASE_NOTES.md` | what this release contains and why |
| `CHANGELOG.md` | concise change list |
| `CLAIM_BOUNDARY.md` | what may / may not be claimed |
| `SHA256SUMS.txt` | checksums of the two release assets |
| `SIGNING_INSTRUCTIONS.md` | exact maintainer steps to sign + publish (you run them) |
| `assets/*.asc` | detached signatures of the assets (added at signing time) |

Binary assets (PDF ~10 MB, DOCX ~4 MB) are attached to the GitHub release, not
committed, following the registry convention used for runtime bundles.

The agent prepared the textual package only — **no signatures, no tag, no release**.
