# CSM Portfolio Intelligence

Customer Success portfolio dashboard and individual account cockpits for a 16-account, $2.09M ARR book of business.

## Architecture

- `docs/index.html` - Portfolio dashboard (entry point, served via GitHub Pages)
- `docs/{account-slug}/index.html` - Individual account cockpits (16 total)
- `data/portfolio.json` - Portfolio data schema (source: Salesforce)
- `data/{account-slug}.json` - Per-account intelligence data

## Features

**Portfolio Dashboard:**
- KPI strip (Total ARR, Avg Engagement, At-Risk, Renewals, Tier 1 count)
- ARR by Product Line (donut chart with account-level tooltips)
- Renewal Timeline (scatter with abbreviated account labels)
- Team Coverage (hover tooltips showing role + specific accounts covered)
- Sortable/filterable account table with engagement bars and risk badges

**Account Cockpits (coming):**
- Account vitals (ARR, products, renewal, contract terms)
- Team coverage map (CSM, AM, EPM, Support, SC)
- Engagement health timeline
- Risk signals and renewal strategy
- Expansion opportunities
- Key contacts and stakeholder map

## Deployment

GitHub Pages from `docs/` directory on `main` branch.

Live at: https://andrewspollard.github.io/csm-portfolio-intelligence/

## Data Sources

- Salesforce (accounts, ARR, contracts, engagement scores, team assignments)
- Chorus (call intelligence - per-account cockpits)
- ZoomInfo (contact enrichment - per-account cockpits)
- Knowledge Graph (relationship context)

---

Built with Amazon Quick | Last refreshed: June 1, 2026
