# HighDefinition Studio website

The studio's hub: players pick a project and read its Privacy Policy and Terms of Use.

Live at **https://hdstudio13.github.io/HighDefinitionStudio/** (GitHub Pages, served from `main`).

Plain static HTML and CSS. No build step, no JavaScript, no third-party requests (system fonts only).
`.nojekyll` tells GitHub Pages to serve the files exactly as they are.

```
index.html                              the hub: pick a project, links to each project's legal pages
assets/css/site.css                     the one shared stylesheet
assets/img/                             swj-icon.png, swj-feature.png
single-weapon-journey/index.html        the project page
single-weapon-journey/privacy.html      Privacy Policy
single-weapon-journey/terms.html        Terms of Use
```

## Store links for Single Weapon Journey

- Privacy Policy: https://hdstudio13.github.io/HighDefinitionStudio/single-weapon-journey/privacy.html
- Terms of Use: https://hdstudio13.github.io/HighDefinitionStudio/single-weapon-journey/terms.html

## Editing the Privacy Policy and Terms of Use

Open `privacy.html` or `terms.html` and edit the text between `<!-- BEGIN LEGAL CONTENT -->` and
`<!-- END LEGAL CONTENT -->`. These tags are styled automatically: `h2`, `h3`, `p`, `ul`, `ol`, `table`,
`blockquote`, `strong`, `a`, `hr`, `code`. Update the effective date in the page header and at the end of the text.

## Adding another project

1. Copy the `single-weapon-journey/` folder, rename it, and edit the three pages.
2. In `index.html`, copy the `<article class="card">` block (and the two links in the Legal section and footer),
   and delete the "next one is in the works" placeholder card.

## Local preview

Run `python -m http.server 8766` in this folder and open http://localhost:8766/.
