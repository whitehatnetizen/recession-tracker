# Recession Tracker

Static dashboards tracking leading indicators for a 1973-style global recession,
with US drivers and Australian transmission.

Deployed at: https://whitehatnetizen.github.io/recession-tracker/

## Pages

- **`index.html`** — daily watch. Latest readings for each leading indicator with
  per-indicator threshold bands (green / amber / red), 380-day spark history, and a
  composite read.
- **`history.html`** — long-history view. The same indicators plotted across
  decades, with NBER-dated US recession bands shaded for calibration.
- **`recession-indicators-chart.html`** — supplementary multi-series chart:
  oil, unemployment, and the Dow, 1970–2026, with a speculative central
  scenario for an Australian 1973-grade recession.

## Data sources

Each chart shows its data source inline (FRED, Yahoo Finance, Cotality,
APRA, ABS, RBA, World Bank, Queensland Government CKAN, etc.). All sources are
public and free.

## Stack

- Pure static HTML, no build step required to view.
- Daily-watch page is fully self-contained. History and supplementary pages
  pull Chart.js + chartjs-plugin-annotation from a CDN.
- Pages are regenerated from a private DuckDB pipeline; only the rendered HTML
  is published here.

## Disclaimer

Personal interpretation of public economic data. Not financial advice.
