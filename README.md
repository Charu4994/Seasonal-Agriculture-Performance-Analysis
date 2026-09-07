# Seasonal Agriculture Performance Analysis

## 📌 Project Overview
This project analyses agricultural performance data across three farming seasons — **Kharif, Rabi, and Zaid** — to uncover seasonal patterns, trends, and relationships in crop yield, profitability, resource usage, and environmental conditions.

## 📂 Files in this Repository
| File | Description |
|---|---|
| `seasonal_agriculture_performance_dataset.csv` | Raw dataset — 4,000 farm records across seasons, states, and crops |
| `Seasonal_Agriculture_Performance_Analysis.ipynb` | Jupyter Notebook containing the full analysis, code, and visualizations |
| `README.md` | Project documentation (this file) |

## 📊 Dataset Description
The dataset contains **4,000 records** covering:
- **Seasons:** Kharif, Rabi, Zaid
- **States:** 8 Indian states
- **Crops:** 8 crop types (Rice, Wheat, Maize, Cotton, Sugarcane, Chilli, Groundnut, etc.)
- **Irrigation Methods:** 4 types (Drip, Flood, Sprinkler, Rainfed)
- **Metrics:** Rainfall, temperature, humidity, soil conditions, fertilizer/pesticide use, yield, production, cost, revenue, profit, water usage/efficiency, and disease/pest risk

## ❓ Problem Statement
Agricultural performance is influenced by seasonal variations in environmental conditions, farming practices, and market conditions. This project investigates how performance differs across seasons by identifying meaningful patterns, trends, relationships, and unusual variations in the data.

## 🔍 Analysis Performed
- Data cleaning (missing value imputation using season+crop-wise medians, duplicate checks)
- Outlier investigation (IQR method)
- Univariate, bivariate, and multivariate analysis
- Correlation analysis (identifying key yield/profit drivers)
- Season-wise comparisons of yield, profit, environmental conditions, and resource usage
- Statistical testing (ANOVA) to confirm significance of seasonal differences
- Crop-wise and state-wise profitability breakdowns
- Irrigation method effectiveness comparison
- 4 student-designed deep-dive analyses
- Evidence-based conclusions and recommendations

## 🛠️ Tools & Libraries Used
- Python 3
- pandas, numpy
- matplotlib, seaborn
- scipy (statistical testing)
- Jupyter Notebook

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone <your-repo-link>
   ```
2. Make sure the `.csv` and `.ipynb` files are in the **same folder**.
3. Open the notebook:
   ```bash
   jupyter notebook Seasonal_Agriculture_Performance_Analysis.ipynb
   ```
4. Run all cells: **Kernel → Restart & Run All**.

## 🔑 Key Insights
- **Season significantly affects profitability but not yield** — Zaid (summer) is loss-making on average despite similar yields to other seasons (confirmed via ANOVA, p < 0.0001).
- **Water efficiency — not fertilizer or rainfall — is the strongest driver of yield** (correlation 0.92).
- **Crop choice matters more than season for profitability** — Sugarcane and Chilli are profitable in every season, while Wheat, Rice, and Maize are consistently loss-making.
- **Flood irrigation is the least water-efficient method in every season**, while Drip and Rainfed perform best.
- More than half of all farms in Rabi and Zaid have zero or negative profit (revealed via violin plot), a more serious finding than average profit alone suggests.

## 🙋 Author
Charu Yadav

---
*This project was completed as part of the VOIS AICTE Batch 2026-2027 Data Analytics program.*
