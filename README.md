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
6. [✨ More information](#-more-information)

---
## 📌 Background & Overview
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

## 📂 Dataset Description & Data Structure
The dataset encompasses total revenue figures blended with comprehensive marketing spend information on an extremely granular level.

Key components of the dataset include:
- **Marketing Expenditure:** Tracks Campaign Budgets, Ad Spend (VND), Delivery Status, and core ad metrics such as Impressions, CPM, CPC, CTR, Inboxes, New vs. Old Customers, and Comments.
- **Sales & Product Data:** Includes SKU (Mã Sản phẩm), Product Name (Tên Sản phẩm), Unit Price (Giá bán), and Sales Volume recorded on the Order Management System.
- **Allocated Metrics:** Detailed allocations mapping the ad spend, inbox metrics, and outcomes directly down to the specific Product/SKU level within a campaign (`Tiền đã chạy Theo Sản phẩm`, `Ngân sách Theo sản phẩm`, `CP/KQ Theo AM`, etc.), allowing for precise ROI calculations.

---
## 🧠 Design Thinking Process
### 1️⃣ STAGE 1: EMPATHIZE (Nhìn rộng)

#### 🔹 5W1H Framework
| Question | Analysis |
| :--- | :--- |
| **Who will view this dashboard?** | Senior Leadership, Marketing Directors, Marketing Team, and Data Analysts. (*Key Stakeholder: Marketing Director / Leadership*). |
| **What problem does it solve?** | Bridging the gap between fragmented data (Ads team vs. Sales team) to accurately measure **Real ROI/ROAS down to the SKU level** and identify unstable net margins despite high ad traffic. |
| **When & Where will it be viewed?** | During weekly/monthly performance reviews, budget allocation meetings, and real-time monitoring of campaign anomalies (e.g., early-stop detection). |
| **Why is this analysis needed?** | To optimize marketing budget efficiency. Currently, high marketing costs burn through budgets (often with 0-2 ROAS) without actionable insights into which specific products/SKUs generate actual profit. |
| **How do they make decisions?** | By cross-referencing Ad Spend (VND) with OMS Sales Data (Revenue, Profit Margin) to scale "Star" campaigns and kill underperforming ones. |

#### 🔹 Empathy Map

| Element | Stakeholder Perspective |
| :--- | :--- |
| **Think & Feel** | *"Why are my marketing costs so high, but the net profit so erratic week-over-week?"*<br>Feels frustrated by 'illusory' ad revenue and fears over-dependency on 1-2 star campaigns. Anxious about lack of early-stop automated rules. |
| **See** | Fragmented reports. The Ads team only shows Clicks/Inboxes, while Sales only shows Total Orders. High ad volume but unexpectedly thin profit margins on those specific items. |
| **Say & Do** | *"What are ads actually selling? Are they profitable?"*<br>Demands to know which campaigns to pause and which SKUs to promote. Tries to manually reconcile ad spend with order data. |
| **PAINS (Challenges)** | 1. Fragmented data.<br>2. Budget burn due to "No Early-Stop" disease.<br>3. High Ad Volume but lower Average Order Value (AOV) compared to Direct Traffic.<br>4. Misaligned Ad Focus (budget pushed into low-margin, easy-to-convert items). |
| **GAINS (Opportunities)** | A unified model tying Top-of-Funnel (Impressions/Spend) to Bottom-Funnel (OMS Revenue/Margin). Clear ROAS per SKU allowing for maximized, stable profitability. |

### 2️⃣ STAGE 2: DEFINE POV (Nhìn sâu)

#### 🔹 Northstar Metrics
| Northstar 1: Return on Ad Spend (ROAS) | Northstar 2: Net Profit Margin |
| :--- | :--- |
| **Value to Measure:** The direct return of revenue for every VND spent on ads at the campaign and SKU level. | **Value to Measure:** The actual profitability after accounting for ad spend and COGS. |
| **Delivery Success:** When ROAS consistently meets or exceeds the target threshold without relying on just one "hero" campaign. | **Delivery Success:** When profit is stable, predictable, and not eroded by high-volume/low-margin ad sales. |
| **Formula:** `Total Campaign Revenue / Total Ad Spend` | **Formula:** `(Total Revenue - COGS - Ad Spend) / Total Revenue` |
| **Why:** To prevent "blind spending" and ensure ads actually convert to revenue. | **Why:** Illusory ad revenues don't keep the lights on; profit does. |

#### 🔹 Point of View (POV) Definition & Growth Formula
| POV | Description | Key Focus / Growth Formula Breakdown |
| :--- | :--- | :--- |
| **POV 1: Campaign Health (Macro)** | Evaluating efficiency of marketing budget across campaigns. | **ROAS & CPA.** Breakdown: Spend vs Revenue tracking, Early-stop trigger metrics (identifying ROAS < 2). |
| **POV 2: Sales Quality & Channels** | Comparing the quality of traffic/sales between Ads and Direct sources. | **AOV & Profit Volatility.** Breakdown: Average Order Value (Ads vs Direct), Revenue contribution % by channel. |
| **POV 3: Product / SKU Profitability** | Mapping specific Marketing Spend to actual Product Sales outcomes. | **Margin per SKU & Allocated Spend.** Breakdown: `Tiền đã chạy Theo Sản phẩm`, Revenue per SKU, Hero Products map. |

### 3️⃣ STAGE 3: IDEATE (Ý tưởng & Cấu trúc)

#### 🔹 Dimension Layering (Brainstorming)
- **Layer 0 (Scorecard):** Total Spend, Total Revenue, Overall ROAS, Average AOV, Overall Profit Margin.
- **Layer 1 (1D Breakdown):** ROAS by Campaign, Revenue by Channel (Ads vs Direct), Top 5/Bottom 5 SKUs by Margin.
- **Layer 2 (2D Breakdown):** ROAS by SKU + Category, AOV by Channel + Time (Weekly Volatility).

#### 🔹 Structure Idea (Dashboard Layout)

##### PAGE 1: Campaign Health Check (Executive Overview)
- **Very Important Info:** Total Spend, Total Revenue, Overall ROAS Scorecard.
- **Important Info:** Top "Star" Campaigns vs. Underperforming Campaigns (ROAS < 2 flags for Early-stop).
- **Detailed Info:** Funnel metrics: CPM -> CPC -> CTR -> Inbox/Comments -> Conversions.

##### PAGE 2: Sales Quality & Channel Performance
- **Very Important Info:** AOV Comparison (Ads vs Direct), Net Profit Trend over time.
- **Important Info:** % Revenue Contribution by Channel, Profit Volatility (Week over Week).
- **Detailed Info:** Analyzing the "Illusory Ad Revenue" hypothesis (high volume, low margin).

##### PAGE 3: Product Segmentation (SKU Deep Dive)
- **Very Important Info:** SKU Profit Margin vs. Allocated Ad Spend (`Tiền đã chạy Theo Sản phẩm`).
- **Important Info:** Hero Products landscape (e.g., *Audrey Shirt, Margnet Dress*). Are they Ad-driven or Organic-driven?
- **Detailed Info:** Cost per Outcome (CP/KQ) per SKU, detecting misaligned ad focus.

### 4️⃣ STAGE 4: PROTOTYPE & REVIEW (Đánh giá)

*During Phase 1 of prototype building, evaluate using the following criteria to iterate (Iterate -> Empathize):*

| Review Area | Quality of Information | Actionable Output |
| :--- | :--- | :--- |
| **Campaign Operations** | Are "early-stop" triggers clear? | If No: Redesign visual threshold alerts for bad ROAS. |
| **Cross-Functional Trust** | Can Sales and Ads teams agree on the numbers? | Ensure the data pipeline linking Ad Spend directly to OMS Revenue via SKU is transparent. |
| **Product Strategy** | Do we immediately know which SKU to boost? | Shift charts from simple Bar Charts to Scatter Plots (Margin vs Ad Spend) to spot optimization pockets. |

*Design Thinking stresses iteration! If the dashboard doesn't answer "Why are we losing net profit?", loop back to the Empathize stage to refine the data model mappings.*


---
## 📊 Key Insights & Visualizations

![Image](https://github.com/user-attachments/assets/a45eabe6-3c81-48d2-a2ed-69f2eb8bb281)

![Image](https://github.com/user-attachments/assets/27221cfa-f8e9-4543-a87a-e991630df752)

![Image](https://github.com/user-attachments/assets/86bb0890-c179-43c5-9171-fa3eae776edb)

![Image](https://github.com/user-attachments/assets/2b7dd89c-7deb-4539-8b05-5b52531b2afb)

![Image](https://github.com/user-attachments/assets/9cfb7db1-e313-4c9e-9095-af1694e0e57c)

---
## ✨ More information 
#### 🛠️ Workflow
This project unfolds through an iterative process heavily reliant on stakeholder feedback and data refinement:

* **Round 1: Data Processing & Modeling:** Cleaning raw data (merging Order tables and Marketing Cost tables), handling the complex allocation syntax, building a robust data model, and releasing the initial Prototype Version 1.
* **Round 2: Iterations:** Gathering feedback to iterate on the prototype significantly across at least 3 versions (Upload mapping versions 1, 2, and 3), ensuring visual clarity and logic validation.
* **Round Final:** Polishing the final dashboard, performing dynamic analysis on the insights discovered, drawing tactical recommendations, and presenting via an analytical video walkthrough.
