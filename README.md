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
- `static/images/`: web-ready paper figures
- `static/js/`: small progressive enhancements, if needed
- `paper-source/`: ignored local storage for the unpublished Overleaf archive

The paper metadata and figures were sourced from `final_iros.tex` in the local Overleaf archive. Keep the archive under `paper-source/` so it cannot be committed accidentally.

## Proposed deployment

Use a separate public GitHub repository named `seeing-where-to-deploy` under the `seoyoung1215` account. Configure GitHub Pages to publish from the `main` branch and repository root. The resulting URL will be:

<https://seoyoung1215.github.io/seeing-where-to-deploy/>

The existing `seoyoung1215.github.io` repository should remain the personal homepage.

After reviewing the page and creating the remote repository:

```bash
git add .
git commit -m "Create paper project page"
git remote add origin https://github.com/seoyoung1215/seeing-where-to-deploy.git
git push -u origin main
```

Then enable Pages in the repository settings with `main` and `/ (root)` as the publishing source.

## Template attribution

The visual structure is adapted from [UMI-on-Air](https://umi-on-air.github.io/) and [UMI-on-Legs](https://umi-on-legs.github.io/), based on the [NeRFies](https://nerfies.github.io/) project-page template. See [LICENSE-WEBSITE.md](LICENSE-WEBSITE.md).
