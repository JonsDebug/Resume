# Jonathan Duvall — Portfolio (Rev. B "spec sheet")

Static site, no build step. Files:

- `index.html` — main resume/spec-sheet page
- `roadmap.html` — full interactive Salesforce roadmap board
- `track.html?track=<key>` — per-track pages with Trailhead checklists
- `roadmap-summary-data.js` / `roadmap-track-data.js` — roadmap content data
- `Cert*.jpg` — certification images

## Deploy to GitHub Pages

1. Create a repo and push everything in this folder to the `main` branch (files at repo root).
2. Repo **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Site appears at `https://<user>.github.io/<repo>/`. All paths are relative, so it works at any subpath.

Notes:
- `.nojekyll` disables Jekyll processing (keep it).
- GitHub Pages CDN caches assets ~10 minutes; hard-refresh after pushing changes.
- Progress check-offs save to the browser's localStorage (per device). Resetting is available on the roadmap board.
