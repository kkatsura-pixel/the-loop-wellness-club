# FORMAL SEPARATION CANDIDATE VERIFICATION — 2026-10-31 JST

## Candidate
- Branch: `recovery/formal-trial-separation-2026-10-31`
- Candidate commit: `2b03453004fd6c8c47708e11853604c1f018db7d`
- Baseline: `b6ca61f8d2866fdaf1573e77073a00ecc6934bde`
- Structural recovery baseline: `safety/baseline-2026-10-31-structural` → `b6ca61f8d2866fdaf1573e77073a00ecc6934bde`

## Exact candidate diff
- Modified formal HTML: `index.html`, `about.html`
- Added formal HTML: `services.html`, `experience.html`, `membership.html`, `founder.html`, `invitation.html`, `access.html`
- Added formal-only assets: 10 paths under `site-assets/`
- Deleted paths: 0
- Changed paths total: 18
- `review/` paths changed: 0

## Reference checks
- All eight formal candidate HTML pages have zero `review/` references.
- All copied `site-assets/` files have the same blob SHA as their designated original source.
- No images, videos, CSS, or media bytes were regenerated, recompressed, edited, or replaced.
- No HLS resource was copied because current formal baseline HTML contains no `.m3u8` reference.

## Not yet verified
- Candidate branch is not the GitHub Pages source and therefore is not available for iPad Safari display testing.
- `main` has not changed.
- No formal cutover has occurred.
- Formal iPad Safari confirmation is pending an approved independent preview method.
