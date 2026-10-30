# REVIEW CLASSIFICATION — READ-ONLY — 2026-10-31 JST

## Confirmed categories
| Category | Files | Meaning |
|---|---|---|
| Formal entry | `/index.html`, `/about.html` | User-designated formal pages |
| Current formal-navigation endpoints | `/review/services.html`, `experience.html`, `membership.html`, `founder.html`, `invitation.html`, `access.html` | Directly linked from the formal entry pages because of their current `<base href="./review/">` routing |
| User-designated trials | `/review/index.html`, `/review/about-test.html` | Trial pages explicitly identified by user |
| Unassigned duplicate | `/review/about.html` | Same baseline blob SHA as `/review/about-test.html`; linked by the six current navigation endpoints; not designated as formal or trial |
| No HTML inbound reference | 37 pages listed below | Not linked by any repository HTML file in this audit; role remains unassigned |

## No-HTML-inbound pages
- `/review/activity-playback-proof.html`
- `/review/atmospheric-depth-test.html`
- `/review/cinematic-slow-zoom-test.html`
- `/review/cinematic-triptych-test.html`
- `/review/editorial-reveal-test.html`
- `/review/forest-light-test.html`
- `/review/general-editorial-reveal-test.html`
- `/review/hero-light-test.html`
- `/review/home-performance-baseline-v12.html`
- `/review/home-performance-baseline-v14.html`
- `/review/home-performance-test-v10.html`
- `/review/home-performance-test-v11.html`
- `/review/home-performance-test-v13.html`
- `/review/home-performance-test-v15.html`
- `/review/home-performance-test-v2.html`
- `/review/home-performance-test-v3.html`
- `/review/home-performance-test-v4.html`
- `/review/home-performance-test-v5.html`
- `/review/home-performance-test-v6.html`
- `/review/home-performance-test-v7.html`
- `/review/home-performance-test-v8.html`
- `/review/home-performance-test-v9.html`
- `/review/home-performance-test.html`
- `/review/home-redesign-test.html`
- `/review/ipad-service-copy-fade-test.html`
- `/review/japan-studio-access-test.html`
- `/review/light-shadow-test.html`
- `/review/motion-test.html`
- `/review/philosophy-full-image-test.html`
- `/review/philosophy-shadow-layer-test.html`
- `/review/philosophy-shadow-test.html`
- `/review/scientific-motion-test.html`
- `/review/screening-video-direct-test.html`
- `/review/screening-video-test.html`
- `/review/smartphone-hero-test.html`
- `/review/social-activity-test.html`
- `/review/subtle-image-movement-test.html`

## Safety interpretation
- “No HTML inbound reference” does not mean safe to delete. This audit does not prove that an external bookmark, manual URL, CSS/JS reference, or future approved workflow does not rely on the file.
- No category in this document authorizes deletion, moving, renaming, URL replacement, or role reassignment.
- The six formal-navigation endpoints under `review/` are a confirmed structural dependency and must be migrated before `review/` can become trial-only.
