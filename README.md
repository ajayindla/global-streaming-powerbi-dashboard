# 🎬 Global Streaming Analytics Dashboard

## Overview
A 4-tab interactive Power BI dashboard analyzing global streaming 
platform performance across 10 platforms, 109 countries (2016–2026).
Built with simulated realistic data covering subscribers, revenue, 
churn, MAU, content ratings and geographic reach.

## Tools & Technologies
- **Power BI Desktop** — Dashboard design & visualization
- **DAX** — 10+ custom measures (Market Share, YoY Growth, Churn Rate, ARPU)
- **Power Query** — Data transformation & ETL
- **Star Schema** — Fact + 4 dimension tables, 4 relationships
- **Excel** — Source data (24,352 rows across 5 sheets)

## Key Metrics
| Metric | Value |
|--------|-------|
| Platforms | 10 (Netflix, Spotify, Disney+, HBO Max, etc.) |
| Countries | 109 globally |
| Time Period | 2016 – 2026 |
| Total Data Rows | 24,352 |
| DAX Measures | 10+ |
| Dashboard Tabs | 4 |

---

## Dashboard Preview

### 1. Dashboard Overview
![Dashboard Overview](dashboard_overview.PNG)
> The executive landing page of the dashboard. Features 6 KPI cards 
> showing Total Subscribers, Avg Churn Rate, Total MAU, YoY Growth, 
> Total Revenue and Avg ARPU. Includes a stacked area chart showing 
> subscriber growth from 2016–2026 across all 10 platforms, a donut 
> chart for market share breakdown, Top 5 Movies and Top 5 Shows by 
> views, and a world map showing global subscriber distribution. 
> Interactive slicers for Platform, Year and Country allow full 
> cross-filtering across all visuals.

---

### 2. Platform Overview
![Platform Overview](platform_overview.PNG)
> Deep dive into platform-level performance. Shows subscriber growth 
> trends per platform over time using an area chart with platform-level 
> color coding. The market share donut chart breaks down each platform's 
> share of total global subscribers. A year range slicer allows dynamic 
> filtering to see how market dominance shifted over time — notably 
> Spotify's consistent lead, Netflix's strong growth, and Disney+'s 
> rapid rise after its 2019 launch.

---

### 3. Content Performance
![Content Performance](content_performance.PNG)
> Analyzes content performance across all 10 platforms. Features a 
> Top 10 Shows by Views bar chart (Wednesday, Squid Game, Stranger 
> Things leading) and a Top 10 Movies by Views bar chart (Red Notice, 
> Don't Look Up, Extraction leading). A genre breakdown donut chart 
> shows the most popular content categories. An IMDb Rating by Platform 
> bar chart reveals that Apple TV+ and HBO Max produce the 
> highest-rated content despite smaller subscriber bases. Platform 
> slicer allows filtering to see content performance per platform.

---

### 4. Global Reach
![Global Reach](global_reach.PNG)
> Geographic analysis of streaming platform penetration worldwide. 
> A filled map visual shades all 109 countries by subscriber volume — 
> darker shading indicates higher subscriber concentration. The United 
> States dominates with the highest subscriber count, followed by 
> the UK, Germany, India and Brazil. A Top 10 Countries bar chart 
> provides a ranked view. Platform and Year slicers allow exploration 
> of which platforms lead in specific regions and how geographic 
> reach expanded over the decade.

---

## Data Model
Star schema with 1 fact table and 4 dimension tables:
- **Fact_Subscribers** — 23,980 rows (core metrics)
- **Dim_Platforms** — 10 platforms
- **Dim_Countries** — 109 countries
- **Dim_Content** — 121 titles
- **Dim_Date** — 2016–2026 date table

## DAX Measures
- Total Subscribers (M)
- Total Revenue (M)
- Avg ARPU
- Avg Churn Rate %
- Total MAU (M)
- YoY Growth %
- Market Share %
- Total New Subscribers (M)
- Total Churned (M)
- Net Subscriber Growth (M)

## Author
**Ajay Indla** | Data Analyst  
📧 Connect on LinkedIn  
🌐 github.com/ajayindla
