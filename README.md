# E-Commerce Platform · KPI Dashboard

A single-file BI dashboard tracking traffic, retention, behavior, RFM segmentation, product heatmaps, and conversion funnels across a **People–Product–Platform** framework.

**Live:** https://ww532.github.io/ecommerce-kpi-dashboard/

## What this is

The original project was built on **SQL + Tableau** over CRM and transaction data. This repo is a rebuilt visualization layer — a self-contained HTML file using Chart.js and Tailwind CSS v4, so the output travels with the link.

## Stack

- Tailwind CSS v4 (browser CDN, `@theme` tokens, full dark mode)
- Chart.js 4
- Geist + Geist Mono
- Vanilla JS — no build step

## Local preview

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

Or just open `index.html` directly in a browser.

## Structure

Eight reports, each fits in one viewport:

1. **Executive Summary** — north-star KPIs + daily traffic + RFM distribution
2. **Traffic Analysis** — PV/UV dual-axis trend
3. **User Retention** — D1 / D3 cohorts
4. **Behavior Patterns** — hourly activity funnel
5. **User Segmentation** — RFM quadrants
6. **Product Heatmap** — top products + category traffic vs CVR
7. **Category Matrix** — PV × CVR scatter quadrant
8. **Conversion Funnel** — three-step drop-off visualization
