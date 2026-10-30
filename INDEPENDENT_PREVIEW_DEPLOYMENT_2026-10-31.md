# INDEPENDENT PREVIEW DEPLOYMENT — 2026-10-31 JST

## Purpose
Provide an iPad Safari verification URL for the formal/trial-separation candidate without modifying any existing formal page, existing `review/` file, or navigation link.

## Recovery point
- Before-preview baseline branch: `safety/baseline-2026-10-31-preview`
- Baseline SHA: `b6ca61f8d2866fdaf1573e77073a00ecc6934bde`

## Preview commit
- `main` preview commit: `2d5556f40456fcbe45fce42297bcb197595fa094`
- Changed paths: 18 added paths, all under `/recovery-preview/`
- Existing paths modified: 0
- Existing paths deleted: 0
- Existing formal navigation links modified: 0
- Existing `review/` paths modified: 0

## Preview URL
https://kkatsura-pixel.github.io/the-loop-wellness-club/recovery-preview/

## Deployment evidence
- GitHub Pages workflow: `pages build and deployment`
- Run: `41102516571`
- Commit: `2d5556f40456fcbe45fce42297bcb197595fa094`
- Result: `completed / success`

## Pending gate
This confirms only that GitHub Pages deployed the preview. iPad Safari comparison remains required. No formal cutover is authorized until user approval after that confirmation.
