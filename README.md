# powerbi-marketing-analytics-dashboard
# Toy Store Sales Analytics Dashboard
<iframe title="Benjamin_PowerBI_MKT317" width="600" height="373.5" src="https://app.powerbi.com/view?r=eyJrIjoiNmY1YjQ2OGUtNmFhZi00NjY0LTllNDEtMGYzNjllZjBiZjc5IiwidCI6IjIyMTc3MTMwLTY0MmYtNDFkOS05MjExLTc0MjM3YWQ1Njg3ZCIsImMiOjN9" frameborder="0" allowFullScreen="true"></iframe>

A Power BI report analyzing toy store sales performance across product categories, regions, and time. Built as a marketing analytics project for MKT 317.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/status-complete-brightgreen)
![Course](https://img.shields.io/badge/course-MKT%20317-blue)

## Overview

This interactive dashboard turns raw toy store sales data into a single-page executive view that answers the questions a marketing or category manager actually cares about:

- **Where** is revenue coming from geographically?
- **What** product categories drive the top line?
- **When** does demand spike — which months, seasons, and regions?
- **How** has performance trended over time?

## Key Insights Surfaced

| Question | Visualization |
|---|---|
| What is total revenue at a glance? | KPI card |
| Which product types sell the most? | Clustered bar chart (Revenue by Item Type) |
| Where is revenue concentrated geographically? | Azure Map + state-level table (Revenue by State) |
| How does revenue trend over time? | Line chart with Year → Quarter → Month → Day drill-down |
| How do regions compare? | Clustered column chart (Revenue by Region) |
| Is there a seasonal pattern? | Revenue by Season table |

## Tools & Techniques

- **Microsoft Power BI Desktop** — data modeling, DAX measures, report design
- **Azure Maps** — geospatial visualization of state-level revenue
- **Date hierarchy drill-down** — interactive time-series exploration from annual to daily
- **Aggregated measures** — `SUM(Revenue)` as the core metric across dimensional cuts

## Data Model

The report is built on a single fact table, `ToyStore`, with dimensions including:

- `ItemType` — product category
- `StateName` / `Region` — geography
- `Date` — with a built-in year/quarter/month/day hierarchy
- `Season` — seasonal bucketing
- `Revenue` — primary metric

## How to Open

1. Download `Benjamin_PowerBI_MKT317.pbix` from this repo
2. Open it with [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
3. Interact with the visuals — click a bar or map state to cross-filter the rest of the page

> No Power BI license is required to view the file locally.

## Repository Contents

```
powerbi-marketing-analytics-dashboard/
├── Benjamin_PowerBI_MKT317.pbix   # The Power BI report
└── README.md                       # This file
```

## About

Built by **Benjamin Padmoasmolo** as part of a marketing analytics portfolio. This project demonstrates end-to-end BI skills: data ingestion, dimensional modeling, DAX-based measure design, geospatial mapping, and executive-ready dashboard design.

---

*Interested in the underlying analysis or want to discuss marketing analytics roles? Reach out via GitHub.*
