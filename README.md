# Attendance Predictor Dashboard — Phase 2

A single-file, client-side attendance predictor dashboard. No build step, no
dependencies to install — open `index.html` and it runs.

**Stack:** Tailwind (CDN) · Chart.js · Font Awesome · Inter (Google Fonts)

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The dashboard. Served at the site root by GitHub Pages. |
| `attendance_predictor_dashboard_phase_2.html` | Original file, kept for the `phase_2` naming. **Identical content** — if you edit the dashboard, edit `index.html` and re-copy, or they will drift. |

## Running locally

Any static file server works:

```bash
python3 -m http.server 3000
# then open http://localhost:3000/index.html
```

## Deploying to GitHub Pages

`.github/workflows/pages.yml` publishes `index.html` to GitHub Pages on every
push to `arena/01a0e6cb-attendance-predicator-dashboar`.

> **One manual step is still required.** Enabling the Pages site needs repo
> **admin** rights, and the automation token used for this repo only has
> contents-write. Both the token and the workflow's own `GITHUB_TOKEN` get
> `403 Resource not accessible by integration` from `POST /repos/{repo}/pages`.
>
> A repo admin must do this once:
>
> 1. **Settings → Pages → Build and deployment → Source → GitHub Actions**
> 2. Save, then re-run the workflow (Actions → *Deploy to GitHub Pages* → **Run workflow**)
>
> The site will publish to:
> `https://sridharsanstudy-collab.github.io/Attendance-predicator-dashboard/`
