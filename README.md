# CRM Sales Performance Dashboard
### B2B Sales Pipeline Analysis | Power BI | Maven Analytics Dataset

---

## 📋 Project Overview

A comprehensive 6-page Power BI dashboard analyzing **8,800 B2B sales opportunities** from a fictitious computer hardware company. The project covers sales team performance, agent efficiency, quarterly trends, product strategy, and account intelligence — built on a clean Star Schema data model with 15+ custom DAX measures.

> **Data Source:** [Maven Analytics — CRM Sales Opportunities Dataset](https://mavenanalytics.io)  
> **Tool:** Power BI Desktop  
> **Domain:** B2B Sales | CRM | Computer Hardware

---

## 🎯 Business Questions

| # | Question |
|---|----------|
| 1 | What separates top-performing teams from the rest? |
| 2 | Which agents are underperforming — and why? |
| 3 | How did sales momentum shift across quarters? |
| 4 | Which products drive the highest win rates? |
| 5 | Which accounts and sectors generate the most value? |

---

## 💡 Key Findings

- **Win Rate dropped 21%** from Q1 (82%) to Q2 (61%), driven by deal volume — not conversion efficiency
- **Darcel Schlecht** generates **$1.15M** — nearly 9x more than the lowest-performing agent
- **GTX Series** accounts for **73% of total revenue** across all regions
- **GTK 500** is sold exclusively by **Celia Rouche's team** (West Region)
- **June** is the peak month ($1.34M), while **July** is the weakest ($700K)
- **Q2 achieved peak revenue ($3.1M)** despite a sharp Win Rate drop — volume, not efficiency, drove it
- **Technology sector** shows the best balance between Revenue and Win Rate

---

---

## 🔍 Key Insights & Business Analysis

> These insights were derived from analyzing 8,800 sales opportunities across agents, products, sectors, and time periods. Each finding is supported by data and framed around a business decision.

---

### 📌 Insight 1 — Revenue is Dangerously Concentrated in a Single Agent

**Finding:**
Darcel Schlecht alone generates **$1.15M — 11.5% of total company revenue ($10M)**.  
The top 5 agents account for **29.8% of revenue**, while the bottom 5 produce only **8.4% combined**.

| Segment | Revenue | % of Total |
|---------|---------|-----------|
| Top 1 Agent (Darcel) | $1,153,214 | 11.5% |
| Top 3 Agents | $2,085,000 | 20.8% |
| Top 5 Agents | $2,983,000 | 29.8% |
| Bottom 5 Agents | $836,000 | 8.4% |

**Business Risk:**  
If the top agent leaves, the company loses over 10% of revenue overnight — with no evident succession plan visible in the pipeline.

**Action:**  
→ Identify what Darcel does differently (deal size, product focus, close speed).  
→ Build a playbook and replicate across underperforming agents.  
→ Consider revenue caps or team redistribution to reduce single-agent dependency.

---

### 📌 Insight 2 — Q2 Peak Was Built on Volume, Not Quality (Hidden Fragility)

**Finding:**  
Q2 2017 hit peak revenue of **$3.1M (+172% QoQ)** — but Win Rate simultaneously **collapsed from 82% to 61.7%**.  
Q3 and Q4 show continued revenue decline (-3.4%, -6.0%) despite stable Win Rates around 61%.

| Quarter | Revenue | Win Rate | QoQ |
|---------|---------|----------|-----|
| Q1 2017 | $1.13M | 82.1% | — |
| Q2 2017 | $3.09M | 61.7% | +172% |
| Q3 2017 | $2.98M | 61.4% | -3.4% |
| Q4 2017 | $2.80M | 60.3% | -6.0% |

**What this means:**  
Q2 growth was driven by flooding the pipeline with low-quality deals — not by improving conversion. The team chased volume over efficiency. Q1's 82% Win Rate suggests the team can perform at a much higher level, but the Q2 surge masked a structural problem.

**Action:**  
→ Investigate Q1 conditions: Was Q1 a smaller, more selective pipeline?  
→ Set Win Rate floors (e.g., minimum 65%) alongside revenue targets.  
→ Avoid rewarding agents purely on deal count — reward on closed revenue.

---

### 📌 Insight 3 — MG Special is a Pricing Problem Disguised as a Sales Win

**Finding:**  
MG Special has the **highest Win Rate of all products (64.8%)** — yet contributes only **0.4% of total revenue** ($43,768 from 1,223 deals).

| Product | Win Rate | Revenue | Contribution | Price |
|---------|----------|---------|-------------|-------|
| MG Special | **64.8%** | $43,768 | **0.4%** | $55 |
| GTX Plus Pro | 64.3% | $2,629,651 | 26.3% | $5,482 |
| MG Advanced | 60.3% | $2,216,387 | 22.2% | $3,393 |

**What this means:**  
Agents are successfully selling MG Special — but the product is priced so low it barely moves the revenue needle. The company is expending real sales effort on a product that generates almost no return.

**Action:**  
→ Review MG Special pricing — is $55 justified?  
→ Redirect agent focus toward higher-margin products without sacrificing Win Rate.  
→ Consider bundling MG Special with GTX products to increase average deal size.

---

### 📌 Insight 4 — GTK 500 is a Single-Team Risk (and a Missed Opportunity)

**Finding:**  
GTK 500, priced at **$26,768** (the highest-priced product), is sold **exclusively by Celia Rouche's West Region team**.  
No other manager has meaningful GTK 500 revenue. GTK Win Rate also shows the steepest quarterly decline: **Q1: 100% → Q4: 43%**.

**Business Risk:**  
- If Celia's team underperforms, the company has zero coverage on its highest-priced product.  
- GTK 500 Win Rate collapse in Q4 (43%) is a warning sign not visible in aggregate metrics.

**Action:**  
→ Train at least one other regional team on GTK 500.  
→ Investigate Q4 Win Rate collapse — pricing objection? Competitive pressure?  
→ Add GTK 500 coverage as a strategic KPI for the sales leadership team.

---

### 📌 Insight 5 — Marketing Sector Punches Above Its Weight

**Finding:**  
The Marketing sector ranks **6th in revenue ($922K)** but has the **joint-highest Win Rate (64.8%)** — tied with MG Special's overall rate. Finance sector ranks 5th in revenue but has the **lowest Win Rate (61.2%)** among known sectors.

| Sector | Revenue | Win Rate | Opportunity Signal |
|--------|---------|----------|--------------------|
| Marketing | $922K | **64.8%** | ✅ High efficiency |
| Entertainment | $689K | 64.7% | ✅ High efficiency |
| Finance | $951K | 61.2% | ⚠️ Low conversion |
| Retail | $1.87M | 63.1% | 📊 Volume-driven |

**What this means:**  
Marketing and Entertainment sectors show superior conversion rates but lower revenue — likely due to smaller deal sizes or fewer accounts. Finance has the money but agents are losing deals more often.

**Action:**  
→ Allocate more senior agents to Finance to improve Win Rate on high-value opportunities.  
→ Expand Marketing sector account coverage — the conversion efficiency is there.

---

### 📌 Insight 6 — All Three Series Collapsed Simultaneously in Q2 (Systemic Issue)

**Finding:**  
All product series show an identical Win Rate pattern: **Q1 ~82-83%** dropping to **Q2 ~61-64%** with no recovery.

| Series | Q1 WR | Q2 WR | Q3 WR | Q4 WR |
|--------|-------|-------|-------|-------|
| GTX | 82% | 62% | 62% | 60% |
| MG | 83% | 61% | 60% | 60% |
| GTK | 100% | 64% | 67% | 43% |

**What this means:**  
The Win Rate drop was **not product-specific** — it happened across all series simultaneously. This rules out product quality or pricing as the cause. The Q2 pipeline flood was driven by a company-wide push (possibly a sales campaign or quota pressure), not by individual product or market dynamics.

**Action:**  
→ Q1 benchmarks should be the target — 82% Win Rate is achievable.  
→ Any future pipeline expansion should be paired with quality controls.  
→ GTK's Q4 collapse (43%) warrants separate investigation — it diverges from GTX/MG stability.

---

### 📌 Insight 7 — Team Size Doesn't Predict Revenue; Efficiency Does

**Finding:**  
All 6 managers lead exactly **5 agents each**. Yet revenue per agent varies by **2x between the best and worst manager**.

| Manager | Revenue | Win Rate | Rev / Agent |
|---------|---------|----------|------------|
| Melvin Marxen | $2.25M | 62.2% | $450K |
| Summer Sewald | $1.96M | **64.3%** | $393K |
| Cara Losch | $1.13M | **64.4%** | $226K |
| Dustin Brinkmann | $1.09M | 63.0% | **$219K** |

**The paradox:**  
Cara Losch has the **highest Win Rate (64.4%)** but the **lowest revenue per agent ($226K)**. Melvin has the **highest revenue** but **below-average Win Rate (62.2%)**.  
This suggests Cara's team wins deals efficiently but works on smaller deal sizes — while Melvin's team chases larger deals and accepts more losses.

**Action:**  
→ Cara's team needs larger deal opportunities — their conversion efficiency is proven.  
→ Melvin's team needs Win Rate coaching — they have the pipeline volume, not the close quality.



## 🗄️ Data Model

### Star Schema

```
accounts_dim    ──(1)──(*) ──┐
products_dim    ──(1)──(*) ──┤──► sales_pipeline (Fact Table)
sales_teams_dim ──(1)──(*) ──┤
DateTable       ──(1)──(*) ──┘
```

### Tables

| Table | Rows | Key Column | Role |
|-------|------|-----------|------|
| sales_pipeline | 8,800 | opportunity_id | Fact Table |
| accounts_dim | 85 | account | Dimension |
| products_dim | 7 | product | Dimension |
| sales_teams_dim | 35 | sales_agent | Dimension |
| DateTable | Dynamic | Date | Date Dimension |

### Date Table (DAX)
```dax
DateTable = 
ADDCOLUMNS(
    CALENDAR(
        MIN(sales_pipeline[engage_date]),   -- earliest deal start
        MAX(sales_pipeline[close_date])     -- latest deal close
    ),
    "Year",           YEAR([Date]),
    "Month Number",   MONTH([Date]),
    "Month Name",     FORMAT([Date], "MMMM"),
    "Quarter",        "Q" & FORMAT([Date], "Q"),
    "QuarterYear",    "Q" & FORMAT([Date], "Q") & " " & YEAR([Date]),
    "Day",            DAY([Date]),
    "Weekday Number", WEEKDAY([Date], 1),
    "Weekday Name",   FORMAT([Date], "dddd")
)
```

> **Important:** After creating the table, go to **Table Tools → Mark as Date Table → select [Date] column**. Required for Time Intelligence functions (PREVIOUSQUARTER, SAMEPERIODLASTYEAR, etc.) to work correctly.

**Why MIN(engage_date) and MAX(close_date)?**
- `engage_date` = deal start date (earliest = 2016)
- `close_date` = deal close date (latest = 2017)
- This ensures the calendar covers the **full lifecycle** of every deal

---

## ⚠️ Data Limitations & Quality Notes

| Issue | Detail | Handling |
|-------|--------|----------|
| Lost deal values | All Lost deals have close_value = $0 | Used Deal Count instead of Lost Revenue |
| GTXPro price | sales_price = $0 in source data | Noted as data gap |
| Account nulls | 12% of accounts have incomplete data | Created "Unknown" member in dimension |
| Engaging nulls | Some Engaging deals missing account info | Flagged as data quality issue |
| Single year | Data covers 2017 only | YoY analysis unavailable |

### Unknown Account Handling
```
employees        → 0
office_location  → Unknown
subsidiary_of    → Unknown
year_established → Null
sector           → Unassigned
revenue          → 0
```

---

## 📊 DAX Measures

### Core Measures
```dax
Total Revenue = 
CALCULATE(
    SUM(sales_pipeline[close_value]),
    sales_pipeline[Deal Stage] = "Won"
)

Won Deals = 
CALCULATE(
    COUNTROWS(sales_pipeline),
    sales_pipeline[Deal Stage] = "Won"
)

Lost Deals = 
CALCULATE(
    COUNTROWS(sales_pipeline),
    sales_pipeline[Deal Stage] = "Lost"
)

Total Deals = COUNTROWS(sales_pipeline)

Open Opportunities = 
CALCULATE(
    COUNTROWS(sales_pipeline),
    sales_pipeline[Deal Stage] IN {"Engaging", "Prospecting"}
)

Total Pipeline Value = SUM(sales_pipeline[close_value])
-- Note: Includes ALL stages (Won + Lost + Open)
```

### Win Rate Measures
```dax
Win Rate % = 
DIVIDE([Won Deals], [Won Deals] + [Lost Deals], 0)

Lost Rate % = 
DIVIDE([Lost Deals], [Won Deals] + [Lost Deals], 0)

Win Rate vs Avg = 
[Win Rate %] - 
CALCULATE([Win Rate %], ALL(sales_teams_dim))

Overall Win Rate = 
CALCULATE([Win Rate %], ALL(sales_teams_dim))
```

### Performance Measures
```dax
Avg Deal Size = 
CALCULATE(
    AVERAGE(sales_pipeline[close_value]),
    sales_pipeline[deal_stage] = "Won"
)

Avg Close Time = 
CALCULATE(
    AVERAGEX(
        FILTER(sales_pipeline, sales_pipeline[deal_stage] = "Won"),
        DATEDIFF(sales_pipeline[engage_date], sales_pipeline[close_date], DAY)
    )
)

Revenue per Day = 
DIVIDE([Total Revenue], [Avg Close Time], 0)

Revenue Contribution % = 
DIVIDE(
    [Total Revenue],
    CALCULATE([Total Revenue], ALL(products_dim)),
    0
)

Open % = 
DIVIDE(
    CALCULATE(COUNTROWS(sales_pipeline),
              sales_pipeline[deal_stage] IN {"Engaging", "Prospecting"}),
    CALCULATE(COUNTROWS(sales_pipeline), ALL(sales_pipeline[deal_stage])),
    0
)
```

### Time Intelligence
```dax
Revenue PQ = 
CALCULATE([Total Revenue], PREVIOUSQUARTER(DateTable[Date]))

QoQ Growth % = 
VAR CurrentQ = [Total Revenue]
VAR PreviousQ = [Revenue PQ]
RETURN DIVIDE(CurrentQ - PreviousQ, PreviousQ, 0)
```

### Dynamic UX Measures (ISINSCOPE Pattern)

These measures use `ISINSCOPE` to show individual values at agent level and averages at the total row — used in Agent Performance Matrix.

```dax
Win Rate (Dynamic) = 
IF(
    ISINSCOPE(sales_pipeline[sales_agent]),
    [Win Rate %],
    AVERAGEX(VALUES(sales_pipeline[sales_agent]), [Win Rate %])
)

Revenue (Dynamic) = 
IF(
    ISINSCOPE(sales_pipeline[sales_agent]),
    [Total Revenue],
    [Avg Revenue per Agent]
)

Deals (Dynamic) = 
IF(
    ISINSCOPE(sales_pipeline[sales_agent]),
    [Total Deals],
    AVERAGEX(VALUES(sales_pipeline[sales_agent]), [Total Deals])
)

Won Deals (Dynamic) = 
IF(
    ISINSCOPE(sales_pipeline[sales_agent]),
    [Won Deals],
    AVERAGEX(VALUES(sales_pipeline[sales_agent]), [Won Deals])
)
```

### Ranking & Dynamic Labels
```dax
Agent Rank = 
RANKX(
    ALL(sales_pipeline[sales_agent]),
    [Total Revenue],
    , DESC, DENSE
)

Selected Manager Title = 
IF(
    HASONEVALUE(sales_teams_dim[Manager]),
    SELECTEDVALUE(sales_teams_dim[Manager]) & "'s Team Performance",
    "Sales Agents Performance Overview"
)
```

### Segmentation Measures
```dax
Product Category = 
VAR Rev = [Total Revenue]
VAR AvgRev = [Product Average Revenue]
VAR WR = [Win Rate %]
RETURN
SWITCH(
    TRUE(),
    Rev >= AvgRev && WR >= [Product Avg Win Rate], "⭐ Star",
    Rev < AvgRev && WR >= [Product Avg Win Rate], "💎 Opportunity",
    Rev >= AvgRev && WR < [Product Avg Win Rate], "🔴 Risk",
    Rev < AvgRev && WR < [Product Avg Win Rate], "⚠️ Weak"
)

Account Category = 
VAR Rev = [Total Revenue]
VAR AvgRev = AVERAGEX(ALL(accounts_dim[account]), [Total Revenue])
VAR WR = [Win Rate %]
VAR AvgWR = AVERAGEX(ALL(accounts_dim[account]), [Win Rate %])
RETURN
SWITCH(
    TRUE(),
    Rev >= AvgRev && WR >= AvgWR, "⭐ Star",
    Rev < AvgRev && WR >= AvgWR, "💎 Opportunity",
    Rev >= AvgRev && WR < AvgWR, "🔴 Risk",
    "⚠️ Weak"
)
```

### Dynamic Manager Cards
```dax
Top Revenue Manager = 
VAR T = ADDCOLUMNS(VALUES(sales_teams_dim[Manager]),
        "R", CALCULATE([Total Revenue]))
RETURN CONCATENATEX(TOPN(1, T, [R], DESC), sales_teams_dim[Manager], "")

Lowest Revenue Manager = 
VAR T = ADDCOLUMNS(VALUES(sales_teams_dim[Manager]),
        "R", CALCULATE([Total Revenue]))
RETURN CONCATENATEX(TOPN(1, T, [R], ASC), sales_teams_dim[Manager], "")

Most Active Manager = 
VAR T = ADDCOLUMNS(VALUES(sales_teams_dim[Manager]),
        "D", CALCULATE([Deal Count]))
RETURN CONCATENATEX(TOPN(1, T, [D], DESC), sales_teams_dim[Manager], "")

Least Active Manager = 
VAR T = ADDCOLUMNS(VALUES(sales_teams_dim[Manager]),
        "D", CALCULATE([Deal Count]))
RETURN CONCATENATEX(TOPN(1, T, [D], ASC), sales_teams_dim[Manager], "")
```

---

## 📄 Dashboard Pages

---

### Page 0 — Landing Page

**Purpose:** Project introduction and navigation hub

**Content:**
- Project title & description
- Dataset stats (8,800 opportunities, 30 agents, 85 accounts)
- 4 Business questions
- Key findings (5 bullet insights)
- Data model summary (Star Schema)
- Tools & techniques used
- Data limitations
- Page navigation buttons

---

### Page 1 — Executive Overview

**Business Question:** What is the overall health of our sales pipeline?

**Audience:** CEO, Sales Director

**Filters:** Date Range | Sector | Region

**KPI Cards:**
| Card | Value |
|------|-------|
| Total Revenue | $10.01M |
| Open Opportunities | 2,089 |
| Win Rate % | 63.15% |
| Lost Rate % | 36.85% |

**Visuals:**

| Visual | Type | X-Axis / Category | Y-Axis / Values | Key Insight |
|--------|------|-------------------|-----------------|-------------|
| Revenue by Account | Bar Chart | accounts_dim[account] | [Total Revenue] | Top: Kan-code $0.34M |
| Revenue by Sector | Bar Chart | accounts_dim[sector] | [Total Revenue] | Top: Retail $1.87M |
| Regional Performance | Bar Chart | regional_office | [Total Revenue] | West $3.57M |
| Deal Stage Distribution | Donut Chart | deal_stage (Legend) | Count of opportunity_id | Won 48.16% |

**Tooltip — Revenue by Account:**
```
Account Name | Sector | Total Revenue | Win Rate % | Deal Count
```

**Tooltip — Revenue by Sector:**
```
Sector | Total Revenue | Win Rate % | Number of Accounts
```

---

### Page 2 — Team & Manager Performance

**Business Question:** What separates top-performing teams from the rest?

**Audience:** Sales Director, VP of Sales

**Filters:** Date Range | Region | Manager

**KPI Cards:**
| Card | Value |
|------|-------|
| Top Revenue Manager | Melvin Marxen |
| Lowest Revenue Manager | Dustin Brinkmann |
| Most Active Manager | Melvin Marxen |
| Least Active Manager | Cara Losch |

**Visuals:**

| Visual | Type | Details | Key Insight |
|--------|------|---------|-------------|
| Revenue vs Efficiency | Scatter Plot | X: Revenue, Y: Win Rate%, Size: Deals, Legend: Manager + Avg Lines | Summer = most efficient |
| Deal Pipeline Distribution | Stacked Bar 100% | Y: Manager, Legend: deal_stage | Win/Loss ratio per manager |
| Revenue Mix by Manager & Product | Stacked Column | X: Manager, Legend: Series | GTK = Celia only |
| Win Rate vs Company Average | Bar Chart | Y: Manager, X: [Win Rate vs Avg] | Diverging colors |

**Drillthrough:** Right-click Manager → Agent Performance Page

**Scatter Plot Avg Lines:**
- Horizontal line: Overall Win Rate = 63.2%
- Vertical line: Avg Manager Revenue

**Tooltip — Scatter:**
```
Manager | Total Revenue | Win Rate % | Deal Count | Avg Deal Size | Avg Close Time
```

**Tooltip — Stacked Bar:**
```
Manager | Deal Stage | Count | % of Row Total
```

---

### Page 3 — Agent Performance

**Business Question:** Which agents are underperforming — and why?

**Audience:** Sales Manager, Team Lead

**Filters:** Date Range | Region | Sector | Account | Manager | Deal Stage

**Navigation:** Drillthrough from Page 2 | "All Agents" button → resets filter

**Dynamic Title:**
```dax
IF(HASONEVALUE(sales_teams_dim[Manager]),
   SELECTEDVALUE(sales_teams_dim[Manager]) & "'s Team Performance",
   "Sales Agents Performance Overview")
```

**Visuals:**

| Visual | Type | Details |
|--------|------|---------|
| Revenue vs Win Rate | Scatter Plot | X: Revenue, Y: Win Rate%, Size: Deals, Legend: Agent + Avg Lines |
| Agent Scorecard | Matrix | See columns below |

**Matrix Columns:**
| Column | Enhancement |
|--------|-------------|
| Rank | Plain number |
| Agent Name | Row label |
| Total Revenue | Data Bars |
| Total Deals | Plain number |
| Win Rate % | Icon (🟢🟡🔴) based on vs Average |
| Avg Close Time | Plain number |
| Avg Deal Size | Plain number |
| Revenue Trend Q1→Q4 | Sparkline |

**Win Rate Icon Rules:**
```
≥ +0% vs Average    → 🟢 Green
≥ -5% and < 0%      → 🟡 Yellow  
< -5% vs Average    → 🔴 Red
```

**Key Insight from Data:**
- Lajuana Vencill: Win Rate 55% (–8.2% vs avg) → Lowest performer
- Darcel Schlecht: $1.15M revenue, Rank #1

---

### Page 4 — Sales Trends & Performance Drivers

**Business Question:** How did sales momentum shift across quarters?

**Audience:** Sales Director, Strategy Team

**Filters:** Date Range | Region

**Visuals:**

| Visual | Type | X-Axis | Y-Axis | Key Insight |
|--------|------|--------|--------|-------------|
| Monthly Revenue Trend | Line Chart | MonthName | [Total Revenue] + Avg Line | Peak: June $1.34M |
| QoQ Revenue Change | Waterfall Chart | QuarterYear | [QoQ Growth %] | Q1→Q2 +172% |
| Win Rate Trend by Series | Line Chart | QuarterYear | [Win Rate %] | GTK volatile |
| Quarterly Revenue Comparison | Column Chart | QuarterYear | [Total Revenue] | Q2 peak $3.1M |
| Win vs Lost Ratio | Stacked Column 100% | QuarterYear | Won + Lost % | Q1 best 82% |

**Tooltip — Monthly Trend:**
```
Month | Total Revenue | Won Deals | Win Rate % | Avg Close Time
```

**Tooltip — Waterfall QoQ:**
```
Quarter | QoQ Growth % | Total Revenue | Won Deals
```

**Insight Box (built into page):**
> *"Q2 achieved peak revenue ($3.1M) despite a sharp drop in win rate from Q1, indicating that deal volume — not conversion efficiency — drove performance. Revenue declined in Q3 and Q4 despite stable win rates, suggesting weaker pipeline activity."*

**Key Numbers:**
| Quarter | Revenue | Win Rate |
|---------|---------|----------|
| Q1 2017 | $1.1M | 82.07% |
| Q2 2017 | $3.1M | 61.7% |
| Q3 2017 | $2.98M | 61.4% |
| Q4 2017 | $2.8M | 60.25% |

---

### Page 5 — Product Strategy & Performance

**Business Question:** Which products drive the highest win rates and where should we focus?

**Audience:** Product Manager, Sales Director

**Filters:** Date Range | Series Slicer | Product Slicer | Region

**Visuals:**

| Visual | Type | Details | Key Insight |
|--------|------|---------|-------------|
| Product Performance Matrix | Scatter Plot | X: Revenue, Y: Win Rate%, Size: Deals, Legend: Series + Avg Lines | 4 Quadrants |
| Revenue by Region & Product | Decomposition Tree | Analyze: Revenue, Explain by: Region → Series → Product | Drill-down |
| Revenue Contribution vs Win Rate | Clustered Bar | Manager + [Revenue Contribution %] + [Win Rate %] | MG Special 0.4% contribution |
| Product Scorecard | Matrix | See columns below | Full comparison |

**Matrix Columns:**
| Column | Enhancement |
|--------|-------------|
| Product | Row label |
| Product Category | ⭐💎🔴⚠️ icon |
| Total Revenue | Data Bars |
| Win Rate % | Color Scale |
| Total Deals | Plain |
| Sales Price | Plain |
| Revenue Contribution % | Plain |
| Win Rate Trend Q1→Q4 | Sparkline |

**Product Quadrant Results:**
| Category | Products |
|----------|---------|
| ⭐ Star | GTXPro, GTX Plus Pro |
| 💎 Opportunity | MG Special |
| 🔴 Risk | MG Advanced |
| ⚠️ Weak | GTX Plus Basic, GTK 500 |

**Key Insight:**
- MG Special: Highest Win Rate (64.8%) but only 0.4% revenue contribution (price = $55)
- GTK 500: Highest price ($26,768) but lowest Win Rate (60%) and only 25 deals

---

### Page 6 — Account Intelligence

**Business Question:** Which accounts and sectors generate the most value — and where are the hidden opportunities?

**Audience:** Account Manager, Sales Director

**Filters:** Region | Sector | Account | Deal Stage

**Visuals:**

| Visual | Type | Details | Key Insight |
|--------|------|---------|-------------|
| Account & Sector Matrix | Scatter Plot | X: Revenue, Y: Win Rate%, Size: Deals, Legend: Sector, Details: Account | Hierarchy view |
| Global Account Map | Map Visual | Location: office_location, Size: Revenue, Color: Win Rate% gradient | Geographic distribution |
| Account Scorecard | Matrix | See columns below | Full detail |

**Map Tooltip:**
```
Account | Sector | Win Rate % | Total Deals | Revenue Contribution | Employees
```

**Scatter Tooltip:**
```
Account | Sector | Total Revenue | Win Rate % | Revenue Contribution | Number of Accounts in Sector
```

**Matrix Columns:**
| Column | Enhancement |
|--------|-------------|
| Account | Row label |
| Account Category | ⭐💎🔴⚠️ |
| Total Revenue | Data Bars |
| Win Rate % | Font Color Scale |
| Total Deals | Plain |
| Sector | Plain |
| Revenue Contribution % | Plain |
| Employees | Data Bars |
| Win Rate Trend Q1→Q4 | Sparkline |

**Key Insight:**
- Technology sector: Best balance between Revenue and Win Rate
- Best performing category: ⭐ Star accounts

---

## 🛠️ Technical Features

| Feature | Implementation |
|---------|---------------|
| Star Schema | 4 Dim Tables → 1 Fact Table |
| Drillthrough | Team Page → Agent Page (filtered by Manager) |
| Dynamic Title | DAX — changes based on Drillthrough context |
| Bookmarks | All Agents / Filter Panel show-hide |
| Tooltip Pages | Custom report page tooltips per visual |
| Sparklines | Revenue trend Q1→Q4 in Matrix visuals |
| Avg Reference Lines | Win Rate & Revenue averages in Scatter plots |
| Conditional Formatting | Data Bars, Color Scale, Icon Rules |
| Time Intelligence | QoQ Growth using PREVIOUSQUARTER() |
| Unknown Member | Null handling for 12% incomplete accounts |
| Page Navigator | Custom navigation on all pages |

---

## ⚠️ Removed / Deprecated Measures

| Measure | Reason |
|---------|--------|
| `Average Revenue` | Duplicate of `Avg Revenue per Agent` |
| `Avg Win Rate` | `Win Rate %` handles context automatically |
| `Open Deals` | Duplicate of `Open Opportunities` |
| `Average Sales Cycle Length` | Bug: returns DateTime not Days — use `Avg Close Time` instead |

## 🔧 Fixed Measures

| Measure | Issue | Fix |
|---------|-------|-----|
| `Agent Revenue Rank` | Used `sales_teams_dim[sales_agent]` | Changed to `ALL(sales_pipeline[sales_agent])` |
| `Lost Rate %` | Missing `,0` in DIVIDE | Added zero-handling |
| `Revenue Manager Contribution %` | Duplicated in model | Removed duplicate |

## 📁 Repository Structure

```
CRM-Sales-Dashboard/
│
├── README.md                          ← This file
├── CRM_Sales_Performance.pbix         ← Power BI file
├── data/
│   ├── sales_pipeline.csv
│   ├── accounts.csv
│   ├── products.csv
│   └── sales_teams.csv
└── screenshots/
    ├── 00_landing_page.png
    ├── 01_executive_overview.png
    ├── 02_team_performance.png
    ├── 03_agent_performance.png
    ├── 04_quarterly_trends.png
    ├── 05_product_strategy.png
    └── 06_account_intelligence.png
```

---

## 👤 Author

Built as a Portfolio Project | Power BI | DAX | Data Modeling

---

*Data Source: Maven Analytics — CRM Sales Opportunities*
