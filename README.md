# Seeing Where to Deploy

Project website for the IROS 2026 paper, "Seeing Where to Deploy: Metric RGB-Based Traversability Analysis for Aerial-to-Ground Hidden Space Inspection."

## Preview locally

From this directory, run:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Structure

- `index.html`: page content and metadata
- `static/css/`: Bulma and project-specific styles
- `static/images/`: web-ready paper figures, portraits, and video poster
- `static/videos/iros26-overview-1080p.mp4`: embedded one-minute overview
- `static/seeing-where-to-deploy.bib`: downloadable citation
- `paper-source/`: ignored local storage for the unpublished Overleaf archive

The paper metadata and figures were sourced from `final_iros.tex` in the local Overleaf archive. Keep the archive under `paper-source/` so it cannot be committed accidentally.

## Deployment

The site is published from the separate `seeing-where-to-deploy` repository under the `seoyoung1215` account:

<https://seoyoung1215.github.io/seeing-where-to-deploy/>

Repository: <https://github.com/seoyoung1215/seeing-where-to-deploy>

The existing `seoyoung1215.github.io` repository remains the personal homepage and is not part of this deployment.

To publish an update from this directory:

```bash
git add .
git commit -m "Update project page"
git push origin main
```

GitHub Pages is configured to publish the `main` branch from `/ (root)`.

To replace the current video later, overwrite `static/videos/iros26-overview-1080p.mp4` with a web-compatible H.264/AAC MP4 and update `static/images/video-poster-1080p.jpg` if needed.

## Design reference

The visual direction was inspired by [UMI-on-Air](https://umi-on-air.github.io/). The implementation is project-specific. See [LICENSE-WEBSITE.md](LICENSE-WEBSITE.md).
