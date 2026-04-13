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
![Image](https://github.com/user-attachments/assets/5503e4ea-0f98-40c0-bcc7-c1d852c3b4e0)
![Image](https://github.com/user-attachments/assets/f27e66f2-d392-42e3-97fc-9510996cd2ef)
![Image](https://github.com/user-attachments/assets/f5e406bc-afb4-4dc4-85ea-c0c4e6bdcbdc)
![Image](https://github.com/user-attachments/assets/3b7948bf-a92b-4309-9c27-13c7c703bdd7)
![Image](https://github.com/user-attachments/assets/1f806f68-79b9-4068-a445-9071bc895925)
![Image](https://github.com/user-attachments/assets/765e8a05-4fe2-4467-8d9a-a9337a39a22f)
![Image](https://github.com/user-attachments/assets/ecca880a-5ab6-4500-8ace-99a3cd8f6613)

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
