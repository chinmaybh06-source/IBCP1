# IBCP 4.0 — Icon-ready package

## What is included
- `index.html`: IBCP dashboard with CSV upload and illustrative demo data
- `icon.png`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`: launcher/browser icons
- `manifest.webmanifest`: install metadata
- `service-worker.js`: basic app-shell caching for repeat visits
- `data/`, `scripts/`, `.github/workflows/`: experimental MoSPI update workflow from the previous package

## Publish to your existing GitHub Pages repository
1. Download and extract this ZIP.
2. Open your repository `chinmaybh06-source/IBCP1` on GitHub.
3. Upload the extracted package contents into the repository root. Merge folders rather than deleting existing repository files. Replace `index.html`; add the icon, manifest, and service-worker files. Keep `.github/workflows/`, `scripts/`, and `data/`.
4. Commit changes to the branch used by GitHub Pages. Wait for the Pages deployment to finish.
5. On Android Chrome, open `https://chinmaybh06-source.github.io/IBCP1/`, tap ⋮, then choose **Install app** or **Add to Home screen**. If you already added it, remove the old shortcut and add it again after the deployment.

## Important notes
- Demo observations are illustrative, not current official economic data. Upload a correctly formatted CSV for your own observations.
- The included MoSPI updater is experimental and its API endpoints/mappings must be validated; do not assume live updates are working just because the workflow exists. The workflow needs a valid `MOSPI_BEARER_TOKEN` GitHub Actions secret.
- GitHub Pages is HTTPS, which supports PWA install features. The exact menu wording depends on your browser version.


Custom branding: the icon files in this package use the user-provided CA India “CA’s can code” logo.
