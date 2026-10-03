# Manan Patel — Portfolio

Personal portfolio website built with [Quarto](https://quarto.org) and hosted on GitHub Pages:
**https://mpp66-ctrl.github.io**

Built for AD688 - Big Data and Cloud Analytics for Business (Boston University, Metropolitan College).

## Pages

| Page | File | Purpose |
|---|---|---|
| Home | `index.qmd` | Introduction, focus areas, and featured work |
| About Me | `about.qmd` | Background, how I work, career goals, and toolbox |
| Projects | `projects.qmd` | Academic projects with descriptions, visuals, and links |
| CV | `cv.qmd` | Summary of my background and a downloadable PDF |
| Contact | `contact.qmd` | Email and GitHub |

## Project structure

```
_quarto.yml        Site configuration (navigation, themes, footer)
theme-light.scss   Light theme variables
theme-dark.scss    Dark theme variables
styles.css         Layout and component styles
assets/            Images (optimized WebP), favicon, and the CV PDF
_design/           Source files used to generate the CV PDF and social card
.github/workflows/ GitHub Actions workflow that publishes the site
```

## Build locally

```bash
quarto preview     # live preview with auto-reload
quarto render      # build the static site into _site/
```

## Deploy

Pushing to `main` runs the **Quarto Publish** GitHub Actions workflow, which renders the site
and publishes it to the `gh-pages` branch served by GitHub Pages.

## Regenerating the CV PDF

`assets/Manan_Patel_CV.pdf` is printed from `_design/cv.html` (Chrome or Edge, "Save as PDF",
headers/footers off, Letter size). Edit the HTML, re-print, and replace the PDF.
