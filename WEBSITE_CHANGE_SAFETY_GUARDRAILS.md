# WEBSITE CHANGE SAFETY GUARDRAILS

## Status
This document is a non-public operational record on the `safety/guardrails-2026-10-31` branch.
It changes no public page and does not change `main`.

## Baseline recovery point
- Baseline date: 2026-10-31 JST
- Protected recovery branch: `safety/baseline-2026-10-31`
- Exact baseline commit: `b6ca61f8d2866fdaf1573e77073a00ecc6934bde`
- Baseline tree: `0e712e5b90c5a48134280a805231a7615437a789`

The baseline commit is the full repository state: public files, trial files, shared `review/` files, assets, and configuration in that tree. It must not be deleted or repointed.

## Formal / trial URLs at baseline
| Role | URL | File |
|---|---|---|
| Formal HOME | https://kkatsura-pixel.github.io/the-loop-wellness-club/ | /index.html |
| Formal ABOUT | https://kkatsura-pixel.github.io/the-loop-wellness-club/about.html | /about.html |
| Trial HOME | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/index.html | /review/index.html |
| Trial ABOUT | https://kkatsura-pixel.github.io/the-loop-wellness-club/review/about-test.html | /review/about-test.html |

## Non-negotiable operation rules
1. Before any write: record the live `main` SHA, target file SHA, target URL, intended diff, and items explicitly out of scope.
2. Before any structural change: create a new `safety/baseline-YYYY-MM-DD` branch at the then-current `main` SHA and verify the branch points to that exact SHA.
3. One write may modify only one approved scope. No bulk move, bulk replacement, or deletion.
4. Any unplanned diff in HTML, URL, asset reference, CSS, JavaScript, image, video, HLS, or filter is an immediate stop condition.
5. Structural work must first be made on a non-public branch / non-public trial URL. `main` is not used as a trial surface.
6. GitHub Pages success is not completion. Required evidence: source diff, public URL check, and user iPad Safari check.
7. No statement such as “done,” “correct,” or “no issue” is allowed before all required evidence exists.
8. `review/` must not be deleted, moved, or batch-edited until all formal-page dependencies have been documented, replaced, and verified on iPad Safari.
9. On failure: stop. Do not stack speculative fixes. Compare against the latest approved safety baseline and restore only after user approval.

## Mandatory change record
Every future change must include:
- Baseline SHA and recovery branch
- Target URL / target file / current file SHA
- Exact intended change
- Explicit non-targets
- Actual diff result
- GitHub Pages result
- Public URL result
- iPad Safari result
- If unsuccessful: rollback target and rollback evidence

## Required platform protection before structural migration
The repository has no GitHub rulesets at the time this record was made. Branch protection could not be inspected by the current connection. Before any production-structure migration, repository owner must confirm in GitHub settings that `main` has protections appropriate to the owner’s workflow (at minimum, require a pull request before merge and block force pushes/deletions where available).

## Recovery procedure
1. Stop all writes.
2. Identify the last user-approved safety baseline.
3. Compare current `main` to that baseline.
4. Show the complete proposed restoration diff to the user.
5. Restore only after user approval.
6. Verify source, Pages deployment, public URL, then iPad Safari.
