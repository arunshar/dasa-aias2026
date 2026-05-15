# DASA + Agents 2026

Companion website for the proposed AIAS 2026 workshop:

**Distortion-Aware Spatial AI and Compute-Grounded Spatial Agents for Scientific Discovery**

A full-day workshop submitted to the [AI for Accelerated Research Symposium (AIAS 2026)](https://www.aiasplus.org/), co-organized by the Tianqiao and Chrissy Chen Institute and UC Berkeley CDSS, San Francisco, November 5 to 7, 2026.

## Quick start

Vanilla HTML + CSS. No build step. To preview locally:

```bash
cd /Users/arunsharma/Desktop/dasa-aias2026
python3 -m http.server 8000
# open http://localhost:8000/
```

## Deploy to GitHub Pages

```bash
# one-time setup
gh repo create arunshar/dasa-aias2026 --public --source=. --remote=origin --push

# enable Pages
gh api -X POST /repos/arunshar/dasa-aias2026/pages \
  -f source.branch=main -f source.path=/
```

Site URL after enablement: `https://dasa-aias2026.github.io` (or `https://arunshar.github.io/dasa-aias2026/` depending on the chosen Pages config).

## File layout

```
dasa-aias2026/
  index.html        # Single-page site (anchored sections)
  stylesheet.css    # Two-color minimal palette (navy + orange)
  README.md         # This file
  assets/
    hero.svg        # Inline conceptual diagram
    favicon.svg     # Site icon
  proposal/         # Workshop proposal PDF (export from Google Doc)
```

## Source of truth

The proposal lives in the Google Doc titled "AIAS 2026 Workshop Proposal v2 (Final Submission Draft)". When the doc updates, mirror the changes here in `index.html`.

## License

Site content released CC BY 4.0 unless otherwise marked.
