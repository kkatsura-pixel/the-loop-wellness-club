# FORMAL_CUTOVER_RECORD_2026-10-31

## Scope
Formal separation from `review/` completed on `main`.

## Pre-write recovery point
- Branch: `safety/baseline-2026-10-31-formal-cutover`
- Exact commit: `a50869a96b39a4b68e4fd3e811f871dd052f27af`
- Verified against the live `main` before the write.

## Formal cutover commit
- Commit: `5208b1474e51613a3d773317284a2ff386bd4faf`
- `main` was updated with an expected-SHA lease from `a50869a...`.
- Post-write comparison: `main` is identical to `5208b...`.

## Exact intended and observed diff
- Modified only: `/index.html`, `/about.html`
- Added only: `/services.html`, `/experience.html`, `/membership.html`, `/founder.html`, `/invitation.html`, `/access.html`
- Added only: `/site-assets/` 10 existing-byte-identical assets.
- No deletion.
- No change under `/review/`.
- No change to `/recovery-preview/`.
- All 8 formal HTML files were SHA-identical to the iPad-approved corresponding files under `/recovery-preview/`.
- All 10 formal assets were SHA-identical to their `/recovery-preview/site-assets/` sources.
- Formal HTML `review/` references: 0.
- Formal HTML parent-directory (`../`) navigation references: 0.

## Pending completion gates
- GitHub Pages workflow result: pending retrieval.
- Formal URLs on user iPad Safari: pending confirmation.
- `review/` remains intact; do not delete, move, or batch edit it.
