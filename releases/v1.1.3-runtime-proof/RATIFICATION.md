# Ratification — `v1.1.3-runtime-proof` as CURRENT_RUNTIME

> **Effective on merge of this change by the steward.** Merging records the steward's
> ratification of `v1.1.3-runtime-proof` as the current **runtime** release pointer
> (`CURRENT_RUNTIME`). This is a governance act, not a technical one.

## What this ratifies
- `CURRENT_RUNTIME` -> **`v1.1.3-runtime-proof`** (signed runtime release; tag GOODSIG
  key `8C8CB0D4`, artefacts happ `a485337...` / dna `e18b4de...`, all signatures verified).
- The conductor boots on this signed runtime in the sovereign environment (verified
  2026-06-23, "Conductor ready").

## What this does NOT do (firewall held)
- **`CURRENT_RELEASE` stays `v1.1.2-genesis`.** That pointer tracks the **prose canon**
  release (white paper), which is **unchanged**. Runtime != canon: the runtime pointer is
  kept separate so a runtime increment never silently restates or supersedes the canon.
- It asserts **no** empirical/site validation, value, right, security, or offering. The
  evidence is the **bounded synthetic WP4 B0-B8** proof only (see `CLAIM_BOUNDARY.md`).

## Disclosure (honest governance status)
- Ratified by the **sole active steward** at this time (Permaculture DAO LLC). The canon's
  multi-stakeholder, multi-author ratification is **not yet** satisfied; this runtime
  pointer is therefore **substantially single-steward** and revisable. No silent change;
  adverse outcomes are never deleted.

## Reversal
Reverting `CURRENT_RUNTIME` is a normal governance edit (a commit), not a history rewrite.
The signed tag/release `v1.1.3-runtime-proof` remains immutable regardless.
