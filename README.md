# 👗Project 4: Visualizing Marketing Spend and Sales Performance in Fashion industry via Power BI Analytics

**Domain:**  
Fashion retail. 

![Image](https://github.com/user-attachments/assets/d4c1657b-f445-499a-b93d-41213d2af22b)

Author: Susan Ho  
Date: 2025-12-26  
Tools Used: Power BI  

---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)
6. [💡 Deep dive into Campaign & SKU Optimization](#-deep-dive-into-campaign-&-sku--optimization)
7. [✨ More information](#-more--information)

---
## 1.📌 Background & Overview
The goal of this project is to build an **analytic and tactical dashboard** to help the company's leadership understand their marketing budget expenditure and evaluate the performance of marketing campaigns. By linking sales revenue directly with marketing spend, this report aims to optimize the efficiency of the marketing budget against key KPIs and propose actionable tactics for improvement.

Through this project, we:
- Process marketing and sales data to build a comprehensive data model.
- Construct prototypes, continuously iterating to address stakeholder reporting needs.
- Link performance metrics (CPM, CPC, CTR, Inbox, Comments) with sales figures (Items sold, Revenue).
- Provide analytical conclusions and tactical recommendations to optimize ROI.
  
### 👤 Project Audience
This project is built for:
- **Senior Leadership & Marketing Directors** who need a clear, data-driven view of budget efficiency and ROI across multiple campaigns and SKUs.
- **Marketing Team / Analysts** to track granular metrics like Cost per Result, Conversion rate by Campaign and Product, identifying areas for immediate tactical shift.

### 🏢 Business Context and ❓Question 
This enterprise operates within the fashion industry, primarily in retail and e-commerce. The company runs multiple cross-channel marketing campaigns (both online and offline) to drive sales and foster brand equity.  
To ensure resources are utilized effectively, management requires consolidated insights to answer the following business questions:

1. **How efficiently is the marketing budget being spent across campaigns?**
- Purpose: Understanding the overall effectiveness of ad spend at a glance.
- Why it matters: Stakeholders need to know if the allocated budget is generating sufficient engagement and interactions at an optimal cost.
- Data perspective: Track CPM, CPC, CTR, Budget Usage, Total Spend (VND), and Conversations/Comments initiated per campaign.  

2. **What is the direct relationship between marketing spend and product sales?**
- Purpose: Linking top-of-funnel marketing metrics to bottom-line revenue.
- Why it matters: It shows which ad variations and product combinations are actually converting into final orders on the OMS (Order Management System), rather than just generating superficial traffic.
- Data perspective: Assess Total Sold, Attributed Sales, Average Price, and Campaign Revenue linked to individual Product IDs/SKUs.

3. **Which campaigns and SKUs should we scale, and which ones are underperforming?**
- Purpose: Optimizing the marketing portfolio and SKUs to maximize profitability.
- Why it matters: Identifying "Star" campaigns guides future budget allocation, whereas discovering underperforming ads/SKUs curtails resource waste.
- Data perspective: Cost per Outcome (CP/KQ), Inbox/Comment allocations per SKU, and margin calculations.

---

## 2.📂 Dataset Description & Data Structure
The dataset encompasses total revenue figures blended with comprehensive marketing spend information on an extremely granular level.

Key components of the dataset include:
- **Marketing Expenditure:** Tracks Campaign Budgets, Ad Spend (VND), Delivery Status, and core ad metrics such as Impressions, CPM, CPC, CTR, Inboxes, New vs. Old Customers, and Comments.
- **Sales & Product Data:** Includes SKU (Mã Sản phẩm), Product Name (Tên Sản phẩm), Unit Price (Giá bán), and Sales Volume recorded on the Order Management System.
- **Allocated Metrics:** Detailed allocations mapping the ad spend, inbox metrics, and outcomes directly down to the specific Product/SKU level within a campaign (`Tiền đã chạy Theo Sản phẩm`, `Ngân sách Theo sản phẩm`, `CP/KQ Theo AM`, etc.), allowing for precise ROI calculations.

---
## 3.🧠 Design Thinking Process
![Image](https://github.com/user-attachments/assets/5503e4ea-0f98-40c0-bcc7-c1d852c3b4e0)
![Image](https://github.com/user-attachments/assets/f27e66f2-d392-42e3-97fc-9510996cd2ef)
![Image](https://github.com/user-attachments/assets/f5e406bc-afb4-4dc4-85ea-c0c4e6bdcbdc)
![Image](https://github.com/user-attachments/assets/3b7948bf-a92b-4309-9c27-13c7c703bdd7)
![Image](https://github.com/user-attachments/assets/1f806f68-79b9-4068-a445-9071bc895925)
![Image](https://github.com/user-attachments/assets/765e8a05-4fe2-4467-8d9a-a9337a39a22f)
![Image](https://github.com/user-attachments/assets/ecca880a-5ab6-4500-8ace-99a3cd8f6613)

---
## 4.📊 Key Insights & Visualizations
![Image](https://github.com/user-attachments/assets/a45eabe6-3c81-48d2-a2ed-69f2eb8bb281)

![Image](https://github.com/user-attachments/assets/27221cfa-f8e9-4543-a87a-e991630df752)
This page focuses on the overall financial overview and the efficiency of the advertising budget for May 2024.

Key Metrics: The report highlights an average ROAS (Return on Ad Spend) of 7.67 and a Total Profit of 195.67 million VND

| Metric | Value |
|---|---|
| **Total Ad Spend** | 396,722,738 VND (~397M VND) |
| **Total Revenue** | 4,773,550,000 VND (~4.77B VND) |
| **Ad-Attributed Revenue** | 3,023,450,000 VND (~3.02B VND) |
| **Organic / Direct Revenue** | ~1,750,100,000 VND (~1.75B VND) |
| **Overall ROAS** | **7.67x** |
| **Ad Share of Total Revenue** | **63.3%** |
| **Total Campaigns Tracked** | 175 campaigns |
| **Unique SKUs in Campaigns** | 184 SKUs |

![Image](https://github.com/user-attachments/assets/86bb0890-c179-43c5-9171-fa3eae776edb)
This page dives into classifying the "star" campaigns versus those that are wasting the budget.
#### 1. ROAS Distribution — The "Small Elite" Problem
Across 175 tracked campaigns, ROAS performance follows a highly skewed distribution:
| ROAS Tier | # Campaigns | Total Spend | Assessment |
|---|---|---|---|
| **>10x (Elite)** | Small group | Dominates revenue | Scale immediately |
| **5–10x (Star)** | Minority | Efficient | Protect & grow |
| **2–5x (Decent)** | Moderate | Break-even high | Monitor closely |
| **1–2x (Poor)** | Significant | Burning budget | Pause & audit |
| **<1x (Loss)** | Present | Net negative ROI | Kill immediately |

**Top Performing Campaigns (ROAS >10x):**
- **\*Lisa Dress 5** campaign: **ROAS = 43.67x** | Spend: 4,578,194 VND → Revenue: ~200M VND ➤ Severely under-funded relative to performance
- **\(G\)Margnet Dress** campaign: **ROAS = 17.38x** | Spend: 6,537,964 VND → Revenue: ~114M VND
- **\*Nevin Dress** campaign: **ROAS = 11.65x** | Spend: 7,850,038 VND → Revenue: ~91M VND
- **\*Nalani 2** campaign: **ROAS = 10.93x** | Spend: 7,105,756 VND → Revenue: ~78M VND
- **\*Audrey Shirt 3** campaign: **ROAS = 10.52x** | Spend: 29,613,977 VND → Revenue: ~312M VND ➤ Top overall revenue driver

**Top Budget Spenders (Campaign Spend Leaders):**
- **AUDREY SHIRT LAL new – Op**: 24,171,418 VND (6.1% of total) | CPM: 52,266 | CPC: 10,874
- **AUDREY SHIRT LAL new – Re**: 23,283,353 VND (5.9%) | CPM: 98,295 | CPC: 26,665
- **Tổng hợp 21/4 FLOWERS MAKE MY DAY**: 14,112,695 VND (3.6%) | CPM: 57,970 | CPC: 12,170
- **AVIAN DRESS – Op**: 9,938,456 VND (2.5%) | CPM: 52,530 | CPC: 4,700 ✅ *Lowest CPC = best click efficiency*

#### 2. The "No Early-Stop" Disease (Confirmed by Data)
Several campaigns continued spending VND past the breakeven point with single-digit or sub-1x ROAS. Key symptoms:
- **High CPM outliers detected**: One campaign segment reached CPM of **144,314** and CPC of **43,368** VND — over **4x the average CPC** — with no halt trigger in place.
- **Budget overshoot**: Multiple campaigns show budget utilization **>100%** (daily budget breached), indicating a lack of automated throttling.
- **The May 4th Incident**: The *TH 25/4 ELEGANT AESTHETICS* campaign — which had achieved a strong ROAS on allocated spend — was manually paused prematurely, cutting off an active revenue stream mid-cycle.

#### 3. Concentration Risk — Revenue Fragility
- The **top 3 campaigns** (Audrey Shirt variants + Lisa Dress 5) account for a disproportionate share of total attributed Ad Revenue. Any disruption to this small cluster collapses system-wide revenue.
- **Audrey Shirt** campaigns alone (3 variants) absorbed **~47.6M VND** in spend and generated **~637M VND** in attributed revenue — representing **~21% of total ad-attributed revenue** from a single product line.

![Image](https://github.com/user-attachments/assets/2b7dd89c-7deb-4539-8b05-5b52531b2afb)
This page analyzes the sources of revenue and the efficiency of the advertising conversion funnel.
#### 1. Total Revenue by Sale Source
| Channel | Revenue | AOV | Order Share | Assessment |
|---|---|---|---|---|
| **Admin (Online)** | 4,016,330,000 VND (84.1%) | 1,404,311 VND | ~84% | Primary channel |
| **Unknown / Direct** | 757,220,000 VND (15.9%) | 1,274,781 VND | ~16% | Lower AOV but higher quality |

- **Admin channel** (primarily ad-driven orders entered by sales staff): Higher absolute volume but slightly inflated AOV due to membership-tier pricing.
- **The AOV gap is 10.2%** in favor of Admin, which may be misleading — Direct orders typically carry higher repurchase intent and come without ad acquisition cost.

#### 2. Order Completion Quality
| Status | Count | Share |
|---|---|---|
| ✅ Thành công (Completed) | 2,273 | 65.9% |
| ⏳ Đang xác nhận (Pending) | 389 | 11.3% |
| 🆕 Mới (New) | 113 | 3.3% |
| 📦 Đang đóng gói (Processing) | 80 | 2.3% |
| ❌ Hệ thống hủy (Cancelled) | 1 | <0.1% |
| — Unknown | 593 | 17.2% |

- **17.2% of entries lack a status** — a data quality gap that could mask cancellations or returns.
- The true completion rate of confirmed orders (Thành công) is **65.9%**, suggesting ~34% of orders are in limbo or untracked states.

#### 3. Geographic Revenue Distribution (Top Cities)
| City | Revenue | Share |
|---|---|---|
| **Hà Nội** | 1,735,210,000 VND | **36.4%** |
| **Hồ Chí Minh** | 1,005,060,000 VND | **21.1%** |
| Hải Phòng | 130,790,000 VND | 2.7% |
| Đồng Nai | 127,460,000 VND | 2.7% |
| Bà Rịa – Vũng Tàu | 115,100,000 VND | 2.4% |
| Đà Nẵng | 112,080,000 VND | 2.3% |

- **Hanoi + HCMC = 57.5% of all revenue.** Campaign geo-targeting should be heavily concentrated in these two metros with differential creative strategy per region.

![Image](https://github.com/user-attachments/assets/9cfb7db1-e313-4c9e-9095-af1694e0e57c)
The final page focuses on which specific products and categories are carrying the revenue load for the company.
#### 1. Hero Product Lineup (Total Revenue — Top Performers)
| Product | Total Revenue | Total Qty | AOV | Ads Sales Rev | ROAS |
|---|---|---|---|---|---|
| *Audrey Shirt 3 | 318,500,000 | 325 | 980,000 | 311,640,000 | 10.52x |
| *Lisa Dress 5 | 314,650,000 | 203 | 1,550,000 | 199,950,000 | 43.67x |
| *Audrey Shirt 1 | 200,900,000 | 205 | 980,000 | 193,060,000 | 8.83x |
| *Avian Dress | 156,800,000 | 98 | 1,600,000 | 120,177,581 | 7.38x |
| (G)Margnet Dress | 152,000,000 | 95 | 1,600,000 | 113,600,000 | 17.38x |
| *Audrey Shirt 2 | 139,160,000 | 142 | 980,000 | 132,300,000 | 5.90x |
| *Percy Set | 138,600,000 | 77 | 1,800,000 | — | — |
| **Varena Set | 132,600,000 | 78 | 1,700,000 | 78,200,000 | 7.20x |

#### 2. Category Revenue Breakdown
| Category | Revenue | Share |
|---|---|---|
| Váy Chiết Eo Xoè (A-line Dresses) | 1,487,850,000 VND | **31.2%** |
| Áo Tách Set (Blouses/Tops) | 1,050,940,000 VND | **22.0%** |
| Set Váy Áo (Dress Sets) | 758,980,000 VND | **15.9%** |
| Váy Chiết Eo Ôm (Fitted Dresses) | 489,400,000 VND | 10.3% |
| Váy Suông Xoè (Loose Dresses) | 388,590,000 VND | 8.1% |
| Set Quần Áo (Outfit Sets) | 255,450,000 VND | 5.4% |
| Chân Váy Tách Set (Skirts) | 211,990,000 VND | 4.4% |
| Quần Tách Set (Pants) | 126,750,000 VND | 2.7% |

- **Váy Chiết Eo Xoè alone drives 31.2%** of Total Revenue — yet ad spend allocation across categories is not proportionally weighted toward this dominant category.
- The **Áo Tách Set category** (shirts/blouses — driven by Audrey Shirt variants) contributes 22% of revenue but receives the highest campaign spend concentration, suggesting reasonable alignment here.

#### 3. The Misalignment Problem — Ad Spend vs. Organic Leaders
- **\*Percy Set** (138.6M Total Revenue, AOV 1,800,000) has zero or near-zero Ads Sales attribution — meaning it sells almost entirely via Direct Sales. This is a missed opportunity to amplify an already-proven product.
- **\*Delia Set** (96.2M, AOV 1,850,000) and **\*Lilla Dress 3** (92.4M, AOV 1,650,000) similarly show minimal ad dependency, yet could benefit from targeted support.
- **Core problem**: Media budget concentrates on high-volume/low-AOV items (Audrey Shirts at AOV 980,000) while high-margin Sets and Dresses running organically at AOV 1,700–1,850,000 sit underfunded.

---
## 5.🔎 Final Conclusion & Recommendations
### 🔑 Core Diagnosis: What the Data Tells Us
This analysis consolidates **175 campaigns, 184 SKUs, 3,454 Total Orders, and ~397M VND in ad spend** into a unified performance picture. Three structural problems are driving margin erosion:
**1. Budget Misallocation — Spending Where It's Easy, Not Where It's Profitable**
- The company is over-investing in Audrey Shirt campaigns (AOV = 980,000 VND) which have high volume but the **lowest per-unit margin** in the portfolio.
- Meanwhile, high-margin products like *Percy Set (AOV 1.8M), *Delia Set (AOV 1.85M), and *Lisa Dress 5 (ROAS 43.67x with only 4.6M spend) are receiving a fraction of what their performance warrants.
- **Recommended Action:** Redistribute 20–30% of Audrey Shirt campaign budget toward Lisa Dress 5, Margnet Dress, and Percy Set campaigns. A ROAS-based auto-bidding reallocation model (e.g., if ROAS >10x → increase budget by 30%) should be implemented in the next sprint.
**2. No Stop-Loss Rules — Budget Bleeding on Underperformers**
- Campaigns with ROAS <2x continue to run unchecked, burning budget that could be redirected to star performers.
- One campaign segment ran at CPM 144,314 VND and CPC 43,368 VND — **4.2x the portfolio average CPC** — with no automatic halt.
- **Recommended Action:** Implement a tiered Early-Stop Policy:
  - **If daily ROAS <1.5x after 200K VND spend → Pause immediately**
  - **If 2-day ROAS <2x → Flag for review and budget cap halved**
  - **If CPM >120K for 3+ consecutive days → Auto-stop and report**
**3. Revenue Concentration Risk — Fragility of the "Star" Dependency**
- Top 3 campaigns generate an outsized share of total ad revenue. A single accidental pause (as documented on May 4th for the ELEGANT AESTHETICS campaign) can trigger a revenue cliff.
- **Recommended Action:** Build campaign redundancy — maintain **at least 2 active ad sets per top-performing SKU**, using audience diversification (LAL New vs. Retargeting vs. Interest-based) so no single ad set is a single point of failure.

### 📋 Prioritized Action Roadmap
| Priority | Action | Expected Impact | Timeline |
|---|---|---|---|
| 🔴 P1 | Implement ROAS-based auto-stop rules (<1.5x at 200K spend) | Recover ~15–20% of wasted spend | Immediate |
| 🔴 P1 | Scale Lisa Dress 5 budget (current ROAS: 43.67x is severely underinvested) | +50–80M VND additional revenue/month | This week |
| 🟠 P2 | Launch Percy Set & Delia Set dedicated ad campaigns | Tap high-margin organic demand with paid amplification | Sprint 2 |
| 🟠 P2 | Create redundant ad sets for Audrey Shirt 3 & Avian Dress | Eliminate single-set revenue fragility | Sprint 2 |
| 🟡 P3 | Geo-target campaigns weighted 60:40 toward Hanoi vs. HCMC | Improve cost-efficiency in primary revenue markets | Sprint 3 |
| 🟡 P3 | Investigate 17.2% unstatused Total Orders | Recover missing revenue data; improve reporting accuracy | Sprint 3 |
| 🟢 P4 | Audit CPM >120K campaigns and rebuild creative strategy | Lower impression costs; improve ad quality scores | Ongoing |
| 🟢 P4 | Build AOV segmentation dashboard by Source (Ad vs. Direct) | Identify true profitable channel mix | Ongoing |

### 📊 Expected Business Impact
If the P1 + P2 recommendations are executed together:
- **Cost savings from stopping low-ROAS campaigns:** Est. 40–60M VND/month
- **Revenue gain from scaling Lisa Dress 5 + Margnet Dress:** Est. 80–120M VND/month
- **Net incremental profit improvement estimate:** 120–180M VND/month
- **ROI of this optimization exercise:** >300% return on time investment within 30 days

---
## 6.💡 Deep dive into Campaign & SKU Optimization
### 🌟 Tier 1: Star SKUs — Scale Immediately

#### SKU: *Lisa Dress 5 (HELSDR — Price: 1,550,000 VND)
- **ROAS: 43.67x** — the highest performing SKU in the entire portfolio
- **Ad Spend:** 4,578,194 VND → **Ad Revenue:** 199,950,000 VND
- **Total Revenue:** 314,650,000 VND | Qty Sold: 203 units
- **Insight:** This SKU is **chronically underfunded**. With a 43.67x ROAS, every additional million VND invested should return ~43M VND in revenue. Even at a conservative 20x post-scale ROAS, a budget increase from ~4.6M → 20M VND would yield an additional **~300M VND in attributed revenue**.
- **Recommendation:** Triple the daily budget for Lisa Dress 5 campaigns immediately. Test at 3 audience tiers: LAL New, LAL Expanded, and Retargeting Separate.

#### SKU: (G)Margnet Dress (Price: 1,600,000 VND)
- **ROAS: 17.38x** | Ad Spend: 6,537,964 VND → Revenue: 113,600,000 VND
- **Total Revenue:** 152,000,000 VND | 95 units sold
- **Insight:** Margnet Dress has a strong AOV of 1,600,000 VND and sells well both organically and via ads. Its Total Revenue (152M) exceeds its Ads Sales revenue (113.6M), confirming strong Direct Sales demand that ads can amplify without cannibalizing.
- **Recommendation:** Add a Retargeting campaign layer to capture website visitors and DM inquirers. Maintain at least 2 concurrent ad sets.

#### SKU: *Audrey Shirt 3 (Price: 980,000 VND)
- **ROAS: 10.52x** | Ad Spend: 29,613,977 VND → Revenue: 311,640,000 VND
- **Total Revenue:** 318,500,000 VND | 325 units — **Highest volume product in portfolio**
- **Note:** AOV of 980,000 VND places this in the lower-margin segment. Gross margin estimation (based on similar cost structures in Data5) suggests margin ~18–22%, making it a volume play rather than a premium margin driver.
- **Recommendation:** Continue funding but avoid further budget concentration increases. Instead, use Audrey Shirt's proven messaging/creative as a template for launching higher-margin SKUs (Varena Set, Percy Set).

---

### ⚠️ Tier 2: Underperforming Campaigns — Action Required

#### Campaign Segment: TH 26/4 YOU DESERVE THE MOST BEAUTIFUL THINGS (LAL)
- **CPM: 144,314 VND | CPC: 43,368 VND** — the most expensive clicks in the dataset
- **Total Spend:** 7,431,381 VND (1.9% of portfolio)
- **Diagnosis:** This campaign targets a broad awareness audience ("new LAL") with unclear conversion intent. The high CPM indicates either **poor creative relevance score** or **saturated audience targeting**.
- **Recommendation:** Pause the current creative. Rebuild with product-specific video content. Test a new product angle (testimonial or try-on format). Re-launch with a hard 2-day ROAS floor of 2.0x before scaling.

#### Campaign Segment: AUDREY SHIRT LAL – Re (Retargeting)
- **CPM: 98,295 VND | CPC: 26,665 VND** — 2.5x the average CPC
- **Spend:** 23,283,353 VND (5.9% of total budget)
- **Diagnosis:** Retargeting audiences are likely **over-saturated** — the same audience is being retargeted too frequently, causing CPM inflation and diminishing returns.
- **Recommendation:** Reduce retargeting frequency cap from current (uncapped) to max 2 impressions/user/day. Split retargeting into 3-day window vs. 7-day window segments with separate creative.

---

### 🔄 Tier 3: High-Potential Organic Stars — Activate with Ads

#### SKU: *Percy Set (Price: 1,800,000 VND)
- **Total Revenue:** 138,600,000 VND | 77 units sold | AOV: 1,800,000 VND
- **Ad Attribution:** Near zero — selling entirely organically
- **Why it matters:** This is a **premium AOV product** with proven end-customer demand. If ad spend can achieve even a 5x ROAS (conservative, given the organic baseline), a 5M VND test campaign would yield 25M VND in attributed revenue.
- **Recommendation:** Launch a small test campaign (5M VND/month) with LAL New audience based on existing buyer profiles. Focus creative on lifestyle positioning, not product shots.

#### SKU: *Delia Set (Price: ~1,850,000 VND)
- **Total Revenue:** 96,200,000 VND | 52 units | AOV: 1,850,000 VND — **Highest AOV in top-15**
- **Ad Attribution:** Minimal
- **Recommendation:** Ideal candidate for a premium "style editorial" content campaign. Target Hanoi and HCMC audiences aged 25–35 with interest in fashion/lifestyle.

---

### 📊 SKU Portfolio Matrix: 2x2 Investment Decision Framework

```
                HIGH ROAS (>10x)
                      |
   [SCALE NOW]        |        [SCALE NOW]
   Lisa Dress 5,      |        Margnet Dress,
   Nevin Dress,       |        Nalani 2
   Nalani 2           |
LOW VOLUME __________|__________ HIGH VOLUME
                      |
   [TEST & LEARN]     |        [OPTIMIZE EFFICIENCY]
   Percy Set,         |        Audrey Shirt 3,
   Delia Set          |        Avian Dress,
   (organic only)     |        Danica Dress 2
                      |
                LOW ROAS (<5x)
```

### 🔬 Micro Case Study: TH 25/4 ELEGANT AESTHETICS — The Pausing Mistake

This campaign represents the clearest example of **operational error undermining marketing performance:**

- The campaign was actively running with a tracking ROAS well above the 5x threshold.
- Campaign was manually paused by the operations team (likely interpreting a temporary CPM spike as underperformance).
- **Impact:** Revenue dropped the following days as the campaign's warm audience lost momentum and needed to be re-built from scratch.

**Key Lesson:** Never pause a campaign based on a single-day CPM spike without reviewing 3-day rolling ROAS. Implement a **mandatory 48-hour cool-off review** before any manual campaign pause.

---

### 📐 Recommended KPI Thresholds 

| KPI | Green (Scale) | Yellow (Monitor) | Red (Review/Pause) |
|---|---|---|---|
| ROAS | >5x | 2–5x | <2x |
| CPM | <60,000 VND | 60K–100K | >100,000 VND |
| CPC | <15,000 VND | 15K–30K | >30,000 VND |
| CTR | >1.5% | 0.5–1.5% | <0.5% |
| Budget Usage | 70–95% | 50–70% | <50% or >100% |
| Cost per Inbox | <40,000 VND | 40K–80K | >80,000 VND |

---
## 7.✨ More information 
#### 🛠️ Workflow
This project unfolds through an iterative process heavily reliant on stakeholder feedback and data refinement:
* **Round 1: Data Processing & Modeling:** Cleaning raw data (merging Order tables and Marketing Cost tables), handling the complex allocation syntax, building a robust data model, and releasing the initial Prototype Version 1.
* **Round 2: Iterations:** Gathering feedback to iterate on the prototype significantly across at least 3 versions (Upload mapping versions 1, 2, and 3), ensuring visual clarity and logic validation.
* **Round Final:** Polishing the final dashboard, performing dynamic analysis on the insights discovered, drawing tactical recommendations, and presenting via an analytical video walkthrough.
