# The Nutrient Glossary — دليل المغذيات

An independent, bilingual (English / Arabic) reference for vitamins, minerals and herbs.

**Live:** https://azzubair.ly/nutrient-glossary/

## What it covers

- Adult RDA / AI values and tolerable upper limits (UL)
- Food sources for every nutrient
- Absorption tips and documented drug / nutrient interactions
- A live search of real product labels in the NIH Dietary Supplement Label Database (DSLD v9 API)
- Full right-to-left Arabic layout, dark / light themes, no tracking scripts

## Data sources

- NIH Office of Dietary Supplements (ODS) fact sheets
- NIH National Center for Complementary and Integrative Health (NCCIH)
- MedlinePlus
- NIH Dietary Supplement Label Database (DSLD)

Values are compiled from the sources above and cross-checked; the page is an educational reference only and does not replace advice from a physician or pharmacist.

## Tech

A single self-contained `index.html` — no build step, no framework, no bundler. Fonts come from Google Fonts and jsDelivr; the label search calls the public NIH DSLD API directly from the browser.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080/.

## Rights

Published as a portfolio reference. All rights reserved — the content and code are not licensed for reuse, redistribution or modification without permission.
