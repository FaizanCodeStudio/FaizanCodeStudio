# 📊 Financial Operations Analytics
### Brazilian E-Commerce (Olist) · Revenue Forecasting · Churn Analysis · Profitability

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Orders-30%2C000-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/Customers-9%2C000-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/SQL%20Views-8-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Notebooks-4-red?style=flat-square"/>
  <img src="https://img.shields.io/badge/ML%20Models-6-purple?style=flat-square"/>
</p>

---

## 🎯 Project Overview

A full-stack **Financial Operations Analytics** project built on the **Olist Brazilian E-Commerce dataset**, combining three technologies across four Jupyter notebooks:

| Technology | Role |
|---|---|
| 🐍 **Python** | Data generation, feature engineering, ML modelling |
| 🗄️ **SQLite + SQL** | Data warehouse, 8 analytical views, all KPI queries |
| 📓 **Jupyter** | Interactive analysis, visualisations, narrative reports |

---

## 🖥️ Executive Dashboard

![Dashboard](visualizations/08_executive_dashboard.png)

---

## 📊 Visualizations

| Revenue Forecasting | Churn Analysis |
|---|---|
| ![](visualizations/04_revenue_forecast.png) | ![](visualizations/06_churn_analysis.png) |

| Profitability | RFM Segments |
|---|---|
| ![](visualizations/07_profitability.png) | ![](visualizations/05_rfm_segments.png) |

---

## 🗂️ Project Structure

```
financial-ops-analytics/
├── 📓 notebooks/
│   ├── 01_EDA_SQL_Exploration.ipynb
│   ├── 02_Revenue_Forecasting.ipynb
│   ├── 03_Churn_Profitability.ipynb
│   └── 04_Executive_Dashboard.ipynb
├── 🐍 src/
│   ├── generate_data.py
│   ├── sql_loader.py
│   ├── analysis_utils.py
│   ├── train_models.py
│   └── generate_report.py
├── 🗄️ sql/
│   └── financial_ops_queries.sql
├── 🤖 models/
│   ├── forecast_poly_ridge.pkl
│   ├── forecast_gbm_regressor.pkl
│   ├── churn_gbm_classifier.pkl
│   ├── churn_random_forest.pkl
│   └── model_metadata.json
├── 📊 visualizations/          ← 9 PNG charts
├── 📄 reports/                 ← HTML report
├── run_all.py
└── requirements.txt
```

---

## 🗄️ SQL Views

| View | Purpose |
|---|---|
| `vw_order_financials` | Master join — revenue, margin, delivery |
| `vw_monthly_revenue` | Monthly KPI aggregation |
| `vw_category_profitability` | Category revenue & margin |
| `vw_seller_performance` | Seller scorecard |
| `vw_customer_rfm` | RFM scores + churn flag |
| `vw_state_revenue` | Geographic breakdown |
| `vw_payment_analysis` | Payment type mix |
| `vw_churn_revenue_risk` | Revenue at risk by segment |

---

## 🚀 Quick Start

```bash
git clone https://github.com/FaizanCodeStudio/financial-ops-analytics.git
cd financial-ops-analytics
pip install -r requirements.txt
python run_all.py
```

---

## 🔑 Key Insights

| Dimension | Insight |
|---|---|
| Revenue | 24-month upward trend; seasonal peaks Nov–Dec |
| Top State | SP drives 38%+ of revenue |
| Top Category | `bed_bath_table` by volume |
| Avg Margin | ~84% gross margin |
| Churn Rate | ~43% inactive >180 days |
| Payment Mix | Credit card 74%, boleto 19% |

---

## 👨‍💻 Author

**Mohd Faizan Khan**  
[![GitHub](https://img.shields.io/badge/GitHub-FaizanCodeStudio-181717?style=flat-square&logo=github)](https://github.com/FaizanCodeStudio)

---

## 📄 License

MIT License
