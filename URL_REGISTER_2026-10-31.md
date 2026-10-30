# URL REGISTER — OBSERVED ROUTING — 2026-10-31 JST

## Scope and meaning
Read-only URL inventory derived from the baseline `main` source.
“Observed route” means the current source resolves to that URL. It does **not** authorize a role change, publication change, deletion, or migration.

## Explicitly designated pages
| Role | File | URL | Basis |
|---|---|---|---|
| Formal HOME | `/index.html` | https://kkatsura-pixel.github.io/the-loop-wellness-club/ | User-approved formal root |
| Formal ABOUT | `/about.html` | https://kkatsura-pixel.github.io/the-loop-wellness-club/about.html | User-approved formal public ABOUT |
| Trial HOME | `/review/index.html` | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/index.html | User-designated trial |
| Trial ABOUT | `/review/about-test.html` | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/about-test.html | User-designated trial |

## Current routes exposed by formal HOME and ABOUT navigation
Both formal `/index.html` and formal `/about.html` contain `<base href="./review/">`.
Therefore their relative navigation links resolve as follows:

| Navigation label | Current resolved URL | Source file at endpoint | Role status |
|---|---|---|---|
| HOME | https://kkatsura-pixel.github.io/the-loop-wellness-club/ | `/index.html` | Formal |
| ABOUT | https://kkatsura-pixel.github.io/the-loop-wellness-club/about.html | `/about.html` | Formal |
| SERVICES | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/services.html | `/review/services.html` | Current navigation endpoint; formal/trial role not yet approved |
| EXPERIENCE | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/experience.html | `/review/experience.html` | Current navigation endpoint; formal/trial role not yet approved |
| MEMBERSHIP | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/membership.html | `/review/membership.html` | Current navigation endpoint; formal/trial role not yet approved |
| FOUNDER | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/founder.html | `/review/founder.html` | Current navigation endpoint; formal/trial role not yet approved |
| INVITATION | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/invitation.html | `/review/invitation.html` | Current navigation endpoint; formal/trial role not yet approved |
| ACCESS | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/access.html | `/review/access.html` | Current navigation endpoint; formal/trial role not yet approved |

## Pages not currently assigned a role
- `/review/about.html` is a duplicate-content page with the same baseline blob SHA as `/review/about-test.html`. It is not an endpoint in the formal HOME/ABOUT navigation observed above. Its role is **unassigned**.
- Thirty-six additional `/review/*test*.html`, performance-test, motion-test, and proof pages exist. Their presence does not imply that they are deletable. Their inbound references and asset dependencies will be assessed in the read-only dependency inventory.

## Prohibitions preserved
No URL role, URL path, link, page content, asset, CSS, JavaScript, video, HLS item, or folder was changed while compiling this register.
