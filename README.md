# Telco Customer Churn — Data Analyst Capstone

**Business problem:** The company is losing ~22% of customers to churn. This project identifies which segments churn the most and delivers actionable retention recommendations.

## Repo Structure

| File | Day | Description |
|---|---|---|
| `01_proposal.md` | 1 | Project proposal — dataset, business problem, objectives |
| `02_data_cleaning.ipynb` | 2 | Cleaning & preprocessing notebook |
| `telco_churn_raw.csv` | 2 | Raw dataset |
| `telco_churn_cleaned.csv` | 2 | Cleaned dataset (output of notebook above) |
| `03_eda.ipynb` | 3 | Exploratory data analysis, 6 visualizations |
| `charts/` | 3 | Standalone PNG exports of each EDA chart |
| `04_dashboard.html` | 4 | Interactive filterable retention dashboard (open in any browser) |
| `05_insights_recommendations.md` | 5 | Insights and prioritized recommendations |
| `06_presentation.pptx` | 6 | Final stakeholder presentation (9 slides) |

## Key Findings
- Overall churn rate: **22.3%**
- Month-to-month contract customers churn at **31.4%** — roughly 3x two-year contract customers
- New customers (0–12 months tenure) churn at **29.0%**
- Fiber optic customers churn more than DSL (**27.9%** vs **18.6%**)
- Electronic check payers churn more than autopay users (**28.1%** vs ~19%)

## How to Use
1. Open `04_dashboard.html` in any browser — no server needed, filters and KPIs work client-side.
2. Notebooks (`02_data_cleaning.ipynb`, `03_eda.ipynb`) run top-to-bottom with `pandas` and `matplotlib`.
3. `06_presentation.pptx` opens in PowerPoint, Google Slides, or Keynote.

## Data Note
The dataset used here is a synthetic dataset generated to match the structure and
statistical patterns (columns, churn rate, correlations) of the widely-used
IBM/Kaggle Telco Customer Churn dataset. To reproduce with the original data,
download it from Kaggle and replace `telco_churn_raw.csv` — the cleaning and
analysis pipeline will run unchanged.
