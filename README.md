# 📊 E-Commerce Sales Dashboard

A comprehensive Power BI dashboard analyzing sales performance, profitability, and operational efficiency across a multi-year e-commerce dataset. Built to identify revenue drivers, pinpoint margin leakage, and guide strategic decision-making.

![Overview Dashboard](https://github.com/nyobel/e-commerce_sales_analytics_and_reporting/blob/main/Dashboard%20Images/Overview.png?raw=true)

## 🎯 Project Overview

This dashboard transforms 9,994 transaction records (2014-2017) into actionable insights across four key dimensions:
- **Sales Performance**: Revenue trends, growth patterns, and customer segmentation
- **Product Analysis**: Category profitability, and discount impact
- **Regional Intelligence**: Geographic distribution, margin variance, and operational efficiency
- **Customer Insights**: High-value account identification, churn risk, and lifetime value

**Key Finding**: While revenue grew 51% over 4 years, 18.7% of orders are loss-making due to aggressive discounting (30%+), with the Central region showing the weakest margins (7.92%) despite high discount rates (15.5%).

---

## 📈 Dashboard Pages

### 1️⃣ Overview
**Purpose**: Executive summary with headline KPIs and growth trends

**Key Metrics**:
- Total Sales: $2.3M
- Total Profit: $286.4K (12.5% margin)
- Average Order Value: $459
- Year-over-year growth visualization with profit margin trending

**Key Insights**:
- Sales grew from $484K (2014) to $733K (2017) — **51% growth over 4 years**
- Profit margin improved from 10.2% (2014) to peak of 13.4% (2016), then declined to 12.7% (2017)
- **Furniture is the problem child**: 32% of revenue, only 6% of profit (2.49% margin)
- **Technology drives profitability**: 36% of revenue, 51% of profit (17.40% margin)
- Consumer segment dominates volume (50.6%) but Home Office delivers best margins (14.03%)
**Business Question Answered**: *Are we growing profitably or just growing?*

### 2️⃣ Product Analysis
**Purpose**: Identify profitable vs. loss-making products and optimize assortment

![Overview Dashboard](https://github.com/nyobel/e-commerce_sales_analytics_and_reporting/blob/main/Dashboard%20Images/product_analysis.png?raw=true)

**Visualizations**:
- Profit by sub-category (17 categories ranked)
- Sales volume distribution
- Discount allocation analysis

**Critical Findings**:
- **Loss-makers**: Tables (-$17.7K), Bookcases (-$3.5K), Supplies (-$1.2K)
- **Top performers**: Copiers ($55.6K profit, 37% margin), Phones ($44.5K), Paper (43% margin)
- Tables receive the highest discount dollars yet remain deeply unprofitable
- Bookcases are the second-highest discounted category and also loss-making
- Chairs and Phones receive heavy discounts but remain profitable due to volume
**Business Question Answered**: *Which products should we promote vs. discontinue?*


### 3️⃣ Regional Analysis
**Purpose**: Compare regional performance and identify operational inefficiencies

![Overview Dashboard](https://github.com/nyobel/e-commerce_sales_analytics_and_reporting/blob/main/Dashboard%20Images/regional_analysis.png?raw=true)

**Metrics Tracked**:
- Sales vs. profit by region
- Discount rate % (normalized metric)
- Average order value by geography

**Key Insights**:
- Central region applies **15.5% discount rate** (highest) yet achieves only **7.92% margin** (lowest)
- West applies **12.9% discount rate** (lowest) and achieves **14.94% margin** (highest)
- **Central is over-discounting by ~20% compared to West**, destroying profitability
**Business Question Answered**: *Why do some regions perform better than others?*

### 4️⃣ Customer Analysis
**Purpose**: Segment customers by value and profitability

![Overview Dashboard](https://github.com/nyobel/e-commerce_sales_analytics_and_reporting/blob/main/Dashboard%20Images/customer_analysis.png?raw=true)

**Visualizations**:
- Scatter plot: Sales (X) vs. Profit (Y) with segment color-coding
- Top 5 customer deep-dive
- Segment performance cards

**Notable Findings**:
- **Sean Miller**: #1 by revenue ($25K) but loss-making (-$2K profit) — high-risk account
- **Tamara Chand**: Ideal customer profile ($19K sales, $9K profit, 47% margin)
- Office customers spend more per order ($473) and deliver the best margins (14.03%) despite being the smallest segment. This is the ideal customer profile to replicate.
**Business Question Answered**: *Are our biggest customers actually profitable?*

---

## 🛠️ Technical Implementation

**Tools Used**: 
- Python: EDA
- Power BI Desktop: Dashboard

---

## 💼 Strategic Recommendations

### 1. Fix the Discount Problem (Highest Impact)
**Issue**: Discounts above 30% are universally unprofitable  
**Action**: Implement hard cap at 25% discount; require VP approval for exceptions  
**Expected Impact**: Eliminate loss-making orders, improve margin by 2-3 percentage points

### 2. Central Region Intervention
**Issue**: 15.5% discount rate with only 7.92% margin (47% worse than West)  
**Action**: Audit Central's discount approval process; implement regional discount targets  
**Expected Impact**: Closing half the margin gap to company average = +$38K annual profit

### 3. Product Portfolio Optimization
**Issue**: Tables, Bookcases, and Supplies are net-negative  
**Action**: Eliminate discounts on these categories; consider discontinuing worst-performing SKUs  
**Expected Impact**: +$22K profit recovery

### 4. Replicate Home Office Success
**Issue**: Consumer segment (50% of revenue) has weakest margin (11.55%)  
**Action**: Analyze Home Office buying patterns; promote high-margin products to Consumer segment  
**Expected Impact**: 2 percentage point margin improvement on $1.2M = +$24K profit

### 5. High-Risk Account Review
**Issue**: Sean Miller ($25K revenue, -$2K profit) represents worst customer profile  
**Action**: Review contract terms; implement minimum margin thresholds for large accounts  
**Expected Impact**: Convert loss to break-even = +$2K per problematic account

---

## 📁 Repository Structure
```
├── Dashboard Images/
│   ├── overview.png
│   ├── product_analysis.png
│   ├── regional_analysis.png
│   └── customer_analysis.png
├── E-Commerce Sales Dashboard.pbix 
├── sales_data.csv
├── sales_data_eda.ipynb
└── README.md
```
---

## 👤 Author

**Crystal Achieng**
- LinkedIn: [www.linkedin.com/in/crystalachieng]


