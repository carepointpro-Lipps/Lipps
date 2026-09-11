# LIPPS Admin v2.3

A browser authoring upgrade for the live LIPPS Quarto site.

## What changes
- Branded **LIPPS Admin** application title and logo.
- Content split into logical navigation groups: Site, Epidemiology, Health Communication, Assessment briefs, Methods and Projects.
- Material icons and dividers for faster navigation.
- Week labels now show the actual topic, not only a week number.
- Editorial metadata fields: status, author/owner, last reviewed and next review due.
- LIPPS-styled preview pane.
- Safe custom `.qmd` parser that preserves existing Quarto front matter.
- Live site URL wired to the current GitHub Pages deployment.

## Install into the live repository
From `~/Projects/Lipps` copy the three files in this package into `admin/`, then commit and push.

Do not commit GitHub personal access tokens. The CMS token is stored by the browser, not in `config.yml`.
