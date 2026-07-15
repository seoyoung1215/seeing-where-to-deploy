# Seeing Where to Deploy project-page context

Static project homepage for the IROS 2026 paper "Seeing Where to Deploy: Metric RGB-Based Traversability Analysis for Aerial-to-Ground Hidden Space Inspection."

## Architecture

- `index.html`: all page content, metadata, and section structure
- `static/css/bulma.min.css`: vendored Bulma base styles from the attributed template
- `static/css/index.css`: project-specific responsive layout and visual design
- `static/images/`: web-ready figures derived from the paper source
- `static/js/index.js`: optional lightweight interactions using vanilla JavaScript
- `paper-source/`: ignored unpublished Overleaf source, never commit it by default

## Commands

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Editing rules

- Keep the site static. Do not add a framework, package manager, or build step.
- Preserve relative asset paths so GitHub Pages works under `/seeing-where-to-deploy/`.
- Keep paper, code, and video controls explicitly marked as unavailable until real URLs or files exist. Do not use dead links.
- Use `final_iros.tex` as the metadata source of truth unless the user supplies newer camera-ready text.
- Do not commit `paper-source/` or an Overleaf archive unless the user explicitly decides to publish the source.
- Optimize added media for web delivery while retaining the original files in the ignored paper source.
- Preserve responsive behavior, semantic headings, useful alternative text, keyboard navigation, and reduced-motion support.
- Credit UMI-on-Air as a design reference in the footer and `LICENSE-WEBSITE.md`.
- Do not use em dashes in visible page copy or collaborator responses.

## Proposed deployment

- Repository: `seoyoung1215/seeing-where-to-deploy`
- Branch and source: `main`, repository root
- URL: `https://seoyoung1215.github.io/seeing-where-to-deploy/`
