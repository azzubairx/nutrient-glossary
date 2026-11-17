# The Nutrient Glossary — دليل المغذيات

An independent, bilingual (English / Arabic) reference for vitamins, minerals,
herbs and supplement topics.

**Live:** https://azzubair.ly/nutrient-glossary/

## What it covers

- 88 entries: 13 vitamins, 14 minerals, 53 herbs and botanicals, and 6 topic overviews
  (plus multivitamin/mineral products as a separate category)
- RDA / AI and tolerable upper limits (UL) for **every life stage** — birth through
  70+ years, including pregnancy and lactation where the source reports them
- Food sources, absorption enhancers and inhibitors, deficiency and excess symptoms
- Documented drug and herb interactions, tagged by severity
- Herbs state plainly that no RDA or UL applies, with cited safety notes instead
- A live search of real product labels in the NIH Dietary Supplement Label Database
  (DSLD v9 API)
- Full right-to-left Arabic layout, dark / light themes, no tracking scripts

## Data and verification

Every entry carries its own verification date and next review date. The current
edition was checked on **17 November 2026**, and the next full review is scheduled for
**17 November 2027**. Links are re-checked quarterly.

Each figure and claim links to a named government source with its access date:

- NIH Office of Dietary Supplements (ODS) professional and consumer fact sheets
- NIH National Center for Complementary and Integrative Health (NCCIH)
- MedlinePlus
- NIH Dietary Supplement Label Database (DSLD)

Where sources disagree, the entry states the conflict explicitly and does not pick a
side without evidence. Where a fact could not be verified, the entry says so rather
than guessing or deleting the field. The page is an educational reference only and
does not replace advice from a physician or dietitian.

## Tech

`index.html` is the application shell — no framework, no bundler. The reference data
lives in `data.js`, which the page loads before its own script. Fonts come from Google
Fonts and jsDelivr; the label search calls the public NIH DSLD API directly from the
browser.

## PDF export

The **Export PDF** button builds a dedicated print document: cover, table of contents,
an about-and-verification page, and all 88 entries with their tables, interactions and
sources. It uses A4 pages, starts every entry on a new page, and keeps tables and
blocks from splitting across pages, so the download is complete rather than a clipped
screenshot of the screen layout. The full edition is around 120 pages in each language.

## Run locally

Serve the folder (both files must be reachable):

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080/.

## Rights

Published as a portfolio reference. All rights reserved — the content and code are not
licensed for reuse, redistribution or modification without permission.
