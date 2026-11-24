# ARL Business Intelligence Cockpit

A single self-contained portal over **Akij Resource Ltd's** seven business units (SBUs).

## Overview

The hub (`index.html`) combines:

- **Overview** — aggregate FY26-27 YTD revenue, prior-year revenue, and gross-margin health across all 7 SBUs, with a revenue ranking chart and one-click SBU cards.
- **7 SBU cockpits** — each business unit's full *Product Intelligence Cockpit* (price · margin · SKUs · elasticity · competition · market share · channel · area · growth · promotion · Voice of Customer · people · Direction/Decision/Action), loaded in-place via iframe.

| SBU | Code | BU |
|---|---|---|
| Akij Ispat | ISPAT | 224 |
| Akij Ready Mix Concrete | ARMCL | 175 |
| Akij Essentials | AEL | 144 |
| Akij Building Solutions — Asphalt | ABSL | 220 |
| Akij Commodities | ACL | 221 |
| Akij InfoTech | AITL | 138 |
| AKIJ Telecom | ATL | 241 |

## Structure

```
index.html            # combined portal (overview + navigation)
sbu/
  ispat.html
  readymix.html
  essential.html
  asphalt.html
  commodities.html
  infotech.html
  telecom.html
```

Each `sbu/*.html` is a self-contained cockpit (inline CSS/JS/SVG, no external assets).

## Deploy

Static site — no build step. Import the repository into **Vercel** (or any static host); the root `index.html` is served automatically.

> Figures are extracted from the SBU cockpits as of **24 Nov 2026**.
