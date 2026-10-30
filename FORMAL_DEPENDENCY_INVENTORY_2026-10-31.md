# FORMAL DEPENDENCY INVENTORY — 2026-10-31 JST

## Scope
Read-only inventory of dependencies reachable from current formal entry pages. No source, URL, asset, or folder was changed.

## Confirmed base dependency
Both `/index.html` and `/about.html` contain `<base href="./review/">`. Their relative resources resolve under `/review/` unless explicitly root-relative or using `../`.

## Formal entry file dependencies
| Formal entry | CSS | Images | Videos |
|---|---|---|---|
| `/index.html` | `/review/design.css` | `/review/IMG_4757.jpeg`, `/review/IMG_4859.png`, `/review/IMG_4897.jpeg`, `/assets/IMG_4868.png` | `/review/THE_LOOP_Screening_Reverse_0-7x_2cycles.mp4`, `/review/beauty-loop-v3.mp4`, `/review/social-experience-loop.MP4` |
| `/about.html` | `/review/design.css` | `/review/IMG_5167.png`, `/review/about-couple-trial.jpg` | none detected |

## Current navigation dependency
Formal HOME and ABOUT currently resolve SERVICES, EXPERIENCE, MEMBERSHIP, FOUNDER, INVITATION, and ACCESS to their respective `/review/*.html` endpoints.
Each of those six endpoints references `/review/design.css`, `/review/index.html`, `/review/about.html`, and the same six `review/` subpages.

## Asset existence
Every local dependency listed above exists in baseline tree `0e712e5b90c5a48134280a805231a7615437a789`.

## HLS observation
No `.m3u8` reference occurs in current formal `/index.html`. The third service currently directly references `/review/social-experience-loop.MP4`. This is an observation only and authorizes no media change.

## Consequence
Deleting, moving, or batch-editing `review/` would currently break formal entry pages and/or active navigation. It is prohibited until formal-asset migration is independently tested and approved.
