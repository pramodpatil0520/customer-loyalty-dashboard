# 🏆 IBM Cognos Analytics — Customer Loyalty Dashboard

<div align="center">

![Made with IBM Cognos](https://img.shields.io/badge/Made%20with-IBM%20Cognos%20Analytics-054ADA?style=for-the-badge&logo=ibm&logoColor=white)
![Project Type](https://img.shields.io/badge/Type-BI%20Dashboard-0F9D58?style=for-the-badge)
![Dataset](https://img.shields.io/badge/Dataset-Customer%20Loyalty%20Program-FF6D00?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

> **An interactive business intelligence dashboard built using IBM Cognos Analytics to uncover customer loyalty trends, revenue performance, and segmentation insights from a fictional retail electronics company.**

</div>

---

## 📌 Project Overview

This project was developed as part of the **IBM Data Analyst Professional Certificate** (Course: DA0151EN — IBM Cognos Analytics) on Coursera. Using IBM Cognos Analytics' no-code dashboard interface, the project transforms raw customer loyalty data into actionable business intelligence.

The dashboard is split into **two tabs**:
- **Tab A — Product Sales:** KPI metrics and yearly quantity-sold trends by product line (2016–2020)
- **Tab B — Customer:** Geographic revenue map, city-level cost vs. sales analysis, coupon response patterns, and loyalty-based segmentation

The dashboard answers key business questions such as:
- Which product line leads in quantity sold across years (2016–2020)?
- How does unit cost and quantity sold vary across major global cities?
- Which loyalty tier (Bronze / Silver / Gold / Platinum / Elite / VIP) dominates department sales?
- How do customers respond to coupons across different product lines?
- Where are the highest-revenue regions geographically?

---

## 📊 Dashboard Features & Visualizations

### Tab A — Product Sales

| # | Visualization | Chart Type | Insight |
|---|---|---|---|
| 1 | **Total Quantity Sold** | KPI Metric Card | **396K** units sold overall |
| 2 | **Total Revenue** | KPI Metric Card | **$229M** total revenue |
| 3 | Quantity Sold by Order Year, colored by Product Line | Multi-series Line Chart | TV & Video Gaming peaked in 2019 (~44K); Computers & Home Office grew steadily; most lines dropped in 2020 |

### Tab B — Customer

| # | Visualization | Chart Type | Insight |
|---|---|---|---|
| 4 | Revenue & Quantity Sold by Country / State / Province | Geospatial Map (Mapbox) | Revenue concentration in North America; bubble size shows quantity by lat/long |
| 5 | Quantity Sold and Unit Cost by City | Combo Chart (Bar + Line) | London & Birmingham lead in unit cost; quantity sold follows similar ranking |
| 6 | Quantity Sold by Coupon Response, colored by Product Line | Spiral / Radial Chart | Response patterns differ significantly across Computers, Kitchen Appliances, Photography, Smart Electronics, and TV & Video Gaming |
| 7 | Department Sales by Loyalty Status | Packed Bubble Chart | Computers & Home Office and TV & Video Gaming dominate; loyalty tiers (Bronze, Elite, Gold, Platinum, Silver, VIP) shown by bubble color |

> **Loyalty Tiers in Dataset:** Bronze · Silver · Gold · Platinum · Elite · VIP  
> **Product Lines:** Computers and Home Office · Kitchen Appliances · Photography · Smart Electronics · TV and Video Gaming  
> **Key Cities:** London, Birmingham, Toronto, Los Angeles, Miami, Vancouver, Frankfurt, Montreal, Munchen, Oxford

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| **IBM Cognos Analytics** | Dashboard creation, reporting, and interactive visualizations |
| **IBM Cognos Assistant (AI)** | Natural language query ("show Quantity Sold and City") |
| **CSV Upload (My Content)** | Data ingestion into Cognos |
| **KPI Metric Cards** | High-level business performance tracking |
| **Cognos Filters / Slicers** | Interactive drill-down and dynamic filtering |
| **Packed Bubble Chart** | Multi-dimensional category visualization |

---

## 📂 Dataset Information

### Dataset Name
`CustomerLoyaltyProgram.csv`

### Source
Published by **IBM** as part of the IBM Cognos Analytics sample dataset library for the IBM Developer Skills Network.

### Download Link
```
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0151EN-SkillsNetwork/labs/Final%20Assignment_Cognos/CustomerLoyaltyProgram.csv
```

### Dataset Description
The dataset contains information about customer demographics, coupon programs, and loyalty program participation for a **fictional retail electronics company**. It is designed to simulate real-world BI reporting scenarios.

### Key Columns / Fields

| Column | Data Type | Description |
|---|---|---|
| `Customer Name` | String | Full name of the customer |
| `City` | String | Customer's city of residence |
| `Country` | String | Customer's country |
| `Gender` | Categorical | Male / Female |
| `Age` | Integer | Customer's age |
| `Loyalty Status` | Categorical | Bronze / Silver / Gold / Platinum / Elite / VIP |
| `Product Line` | Categorical | Electronics product category |
| `Quantity Sold` | Integer | Number of units purchased |
| `Revenue` | Float | Revenue generated from the transaction |
| `Coupon Response` | Categorical | Whether customer responded to coupon |

---

## 📁 Repository Structure

```
customer-loyalty-dashboard/
│
├── Dataset/
│   └── CustomerLoyaltyProgram.csv             # Raw dataset (IBM sample)
│
├── Dashboard_PDF/
│   └── Customer_Loyalty_Dashboard.pdf         # Exported Cognos dashboard (PDF)
│
├── Dashboard_Screenshots/
│   └── sales_dashboard.png                    # Tab A — Product Sales (KPIs + line chart)
│   └── service_dashboard.png                  # Tab B — Customer (map, city chart, bubbles)
│
└── README.md                                  # Project documentation (this file)
```

---

## 📈 Skills Demonstrated

- ✅ **Dashboard Development** — Multi-panel interactive dashboards in IBM Cognos Analytics
- ✅ **Business Intelligence Reporting** — KPI card creation and metric tracking
- ✅ **Data Visualization** — Bar, column, bubble, pie, and line chart selection and design
- ✅ **Customer Segmentation Analysis** — Loyalty tier and demographic breakdowns
- ✅ **AI-Assisted Analytics** — Used Cognos Assistant (NLP) for quick visual generation
- ✅ **Interactive Filtering** — Applied dashboard-level filters for drill-down analysis
- ✅ **BI Tool Proficiency** — End-to-end workflow: data upload → modeling → visualization → export

---

## 🔍 Key Business Insights

1. **TV and Video Gaming** was the top-performing product line from 2016–2019, peaking at ~44,000 units in 2019, but saw a sharp decline in 2020 — signalling a potential market shift or supply issue worth investigating.
2. **Computers and Home Office** showed consistent year-over-year growth from 2016 to 2020, overtaking other categories — suggesting rising demand likely accelerated by remote work trends.
3. **London and Birmingham** rank highest in unit cost among all cities, while quantity sold is also concentrated in these cities — indicating a premium customer base in the UK market.
4. **Coupon response rates vary significantly** across product lines, with some categories showing much higher engagement — useful for targeted promotional campaign planning.
5. **North America dominates revenue geographically**, with the highest revenue concentration visible across the US and Canada on the geospatial map.
6. The **packed bubble chart** reveals that Computers & Home Office and TV & Video Gaming are the two largest department sales contributors across all loyalty tiers (Bronze through VIP).

---

## 🚀 How to Reproduce

1. Sign up for a **free IBM Cognos Analytics trial** at [ibm.com/products/cognos-analytics](https://www.ibm.com/products/cognos-analytics)
2. Once inside the platform, click **New → Upload files**
3. Upload the `CustomerLoyaltyProgram.csv` file — it will appear under **My Content**
4. Click **New → Dashboard** and select the uploaded dataset as the data source
5. Drag and drop fields onto panels to recreate the visualizations listed above
6. Add KPI cards, apply filters, and use **Cognos Assistant** for AI-generated visuals
7. Export the completed dashboard as a **PDF** via the share/export option

---

## 📜 Course Information

| Field | Details |
|---|---|
| **Platform** | Coursera |
| **Certificate** | IBM Data Analyst Professional Certificate |
| **Course** | Data Visualization and Dashboards with Excel and Cognos (DA0151EN) |
| **Offered by** | IBM |

---

## 🙋 About This Project

This project was completed as the **Final Assignment** for the IBM Cognos Analytics module. It demonstrates the ability to:
- Connect data sources in IBM Cognos
- Build multi-visualization dashboards without writing code
- Extract business insights through visual storytelling
- Present analytics findings in a professional dashboard format

---

---

## 👤 About Me

**Pramod Patil** — Final year Electronics & Telecommunications Engineering student at R.C. Patel Institute of Technology, Shirpur, building hands-on skills in Data Analysis and Machine Learning.

| | |
|---|---|
| 📧 Email | [pramodpatil0520@gmail.com](mailto:pramodpatil0520@gmail.com) |
| 🔗 LinkedIn | [linkedin.com/in/pramod-patil-a00309265](https://www.linkedin.com/in/pramod-patil-a00309265) |
| 🐙 GitHub | [github.com/pramodpatil0520](https://github.com/pramodpatil0520) |

> 🚀 **Open to fresher and internship opportunities in Data Analytics / Data Science.**

---

<div align="center">

Made with ❤️ using IBM Cognos Analytics

</div>
