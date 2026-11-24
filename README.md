# Database of Databases

A curated catalog of **220 rare and obscure publicly accessible databases and archives** — plus **313 tools and resources** for exploring, transforming, visualizing, and publishing the data they contain.

This is the raw material for a content operation that turns obscure datasets into compelling visual content: fun facts, interactive explorations, data art, and infographics.

---

## What's Inside

### 📁 Databases & Archives (`data/databases.json`)

220 verified entries spanning domains like:

- **Historical & Archival** — CIA CREST declassified files, Old Bailey Online criminal records (1674–1913), London Bills of Mortality
- **Scientific & Environmental** — NASA Exoplanet Archive, Global Biodiversity Information Facility, Ice Core Gateway
- **Cultural & Linguistic** — Endangered Languages Project, Alan Lomax Archive, Vatican Apostolic Library digitized manuscripts
- **Geospatial & Earth Science** — USGS Earthquake Hazards, OpenTopography, Global Volcanism Program
- **Biological & Medical** — WHO Mortality Database, MorphoSource 3D specimens, Protein Data Bank
- **Space & Astronomy** — Gaia Star Catalog, Lunar Reconnaissance Orbiter, Minor Planet Center
- **Social & Economic** — World Inequality Database, Global Terrorism Database, GDELT Project

Each entry includes: name, URL, status, operator, country, year established, domain, description, scale, data formats, access model, API availability, content hooks, viral potential, visual potential, and confidence level.

### 🛠 Tools & Resources (`data/tools.json`)

313 entries across four categories:

| Category | Count | Description |
|---|---|---|
| **Data Exploration & Cleaning** | 88 | Tools for discovering what's inside a dataset, cleaning it, reshaping it — from OpenRefine to Astropy to Tesseract OCR |
| **Data Visualization** | 99 | Frameworks for static, interactive, and animated visualizations — from D3.js to Manim to ParaView |
| **Creative Data Resources** | 65 | Assets for compelling content: basemaps, color palettes, icon libraries, public domain archives, inspiration galleries |
| **Publishing & Distribution** | 61 | Infrastructure for turning visualizations into web content: SSGs, CMS platforms, newsletter tools, analytics |

Each entry includes: name, URL, category, type, language/platform, license, status, maturity, description, best-for use case, limitations, learning curve, data scale, input/output formats, composability, API/CLI availability, notable integrations, visual quality, customization depth, export options, and confidence level.

---

## Data Format

Both datasets are available as JSON (primary) and CSV (flat export).

### Database Schema

```json
{
  "name": "Old Bailey Online",
  "url": "https://www.oldbaileyonline.org",
  "status": "Active",
  "operator": "University of Sheffield / Open University",
  "country": "United Kingdom",
  "year_established": "2003",
  "domain": "Historical & Archival",
  "description": "Fully searchable digitization of 197,745 criminal trials held at London's central criminal court from 1674 to 1913...",
  "scale": "197,745 trial records",
  "data_formats": "XML, API, full-text search",
  "access_model": "Free, open access",
  "api_available": "Yes",
  "one_line_hook": "Nearly 200,000 criminal trials spanning 240 years of London justice",
  "viral_potential": "High",
  "visual_potential": "High",
  "confidence": "High"
}
```

### Tools Schema

```json
{
  "name": "D3.js",
  "url": "https://d3js.org",
  "category": "Data Visualization",
  "type": "Library",
  "language_platform": "JavaScript (Web/Browser)",
  "license": "ISC",
  "status": "Active",
  "maturity": "Established",
  "description": "The foundational JavaScript library for custom data-driven visualizations on the web...",
  "best_for": "Highly customized, interactive web-based data visualizations",
  "limitations": "Steep learning curve; no built-in high-level charts",
  "learning_curve": "High",
  "composability": "High",
  "api_cli_available": "Yes",
  "visual_quality": "Publication-ready",
  "confidence": "High"
}
```

---

## Google Sheets

Live versions are maintained in Google Sheets for browsing and filtering:

- [Database of Databases](https://docs.google.com/spreadsheets/d/1nXH8I7BrAVxk3J6KMiAWnXBVcIm05HvwVKKNT6IxlNk/edit) — 220 entries, 20 columns
- [Tools & Resources Catalog](https://docs.google.com/spreadsheets/d/1g4I8flIR3zVVBcoYnGiLWQPXpM01UxlPBLxaKlfWdRw/edit) — 313 entries, 23 columns

---

## Stats

| Metric | Value |
|---|---|
| Total databases cataloged | 220 |
| Total tools cataloged | 313 |
| Combined entries | 533 |
| Open-source tools | 262 (84%) |
| Actively maintained tools | 282 (90%) |
| Countries represented (databases) | 30+ |
| Domains covered | 15+ |

---

## Use Cases

- **Content creation** — Use the databases as source material for daily facts, visualizations, and data stories
- **Tool selection** — Find the right tool for a specific data format, visualization type, or publishing workflow
- **Pipeline design** — Identify tool chains (e.g., DuckDB → Altair → Observable → Astro) for automated content pipelines
- **Education** — Explore unusual datasets for teaching data literacy, visualization, or digital humanities
- **Research** — Discover niche archives that most researchers don't know exist

---

## Project Context

This repository is part of a research series by [Gumdrop Media](https://github.com/williamrthomas):

1. **Assignment 1** — Catalog 150+ rare databases and archives (this repo: `data/databases.json`)
2. **Assignment 2** — Catalog 200+ tools and resources for the data pipeline (this repo: `data/tools.json`)
3. **Reader Personas** — 10 audience profiles for content derived from these databases

---


## Public Data APIs (Apify)

- [USAspending Awards Scraper](https://apify.com/publicrecords/usaspending-awards-scraper) - US federal contract and grant awards by agency, recipient, NAICS and period (Apify Actor, API + MCP).
- [Grants.gov Scraper](https://apify.com/publicrecords/grants-gov-scraper) - Open US federal grants: agency, deadline, eligibility and source link (Apify Actor, API + MCP).
- [Federal Contracts Feed (SAM.gov + Grants.gov)](https://apify.com/publicrecords/govcon-opportunity-feed) - New US federal contract and grant notices from SAM.gov and Grants.gov in one feed (Apify Actor, API + MCP).
- [EU TED Tenders Scraper](https://apify.com/publicrecords/eu-ted-notices-scraper) - EU procurement notices from TED: buyer, CPV, value, deadline, link (Apify Actor, API + MCP).
- [UK Tenders Scraper](https://apify.com/publicrecords/uk-find-a-tender-scraper) - UK government tenders from Find a Tender and Contracts Finder: buyer, value, deadline (Apify Actor, API + MCP).
- [City Council Meetings Scraper (Legistar)](https://apify.com/publicrecords/legistar-meetings-scraper) - City council meetings, agenda items and documents for any Legistar city (Apify Actor, API + MCP).
- [Calibration Ledger](https://apify.com/publicrecords/calibration-ledger) - Forecast track records (IMF, OECD, Fed, ECB SPF): forecast errors and bias by organization (Apify Actor, API + MCP).

## License

The catalog data in this repository is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The databases and tools referenced retain their own respective licenses.

---

## Contributing

Found a database we missed? Know a tool that belongs here? Open an issue or submit a PR with new entries following the existing schema.
