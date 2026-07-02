# Capstone Project Proposal: Customer Churn Analysis for a Telecom Company

## 1. Dataset
**Source:** Telco Customer Churn dataset (IBM sample data, structure matches the
widely-used Kaggle dataset: https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

**Size:** ~7,000 customer records, 21 columns

**Description:** Each row represents a customer at a telecom company, with:
- Demographics (gender, senior citizen status, partner, dependents)
- Account information (tenure, contract type, payment method, billing)
- Services subscribed to (phone, internet, streaming, security add-ons)
- Charges (monthly charges, total charges)
- Target variable: `Churn` (Yes/No)

## 2. Business Problem
> **"The company is losing approximately 1 in 4 customers to churn. Which customer
> segments are most likely to churn, and what specific, actionable steps can the
> retention team take to reduce churn rate?"**

This matters because acquiring a new customer typically costs far more than
retaining an existing one — even a small reduction in churn has an outsized
effect on recurring revenue.

## 3. Objectives
1. Identify the top 3–5 factors most strongly associated with customer churn.
2. Segment customers into risk groups based on those factors.
3. Quantify the revenue impact of churn in the highest-risk segments.
4. Deliver specific, actionable retention recommendations tied to the data.

## 4. Project Goals & Real-World Alignment
This mirrors a real task a business/data analyst on a retention or customer
success team would be asked to do: turn raw account data into a dashboard
and a short set of recommendations that a non-technical manager can act on
within a quarter.

## 5. Approach / Plan
| Day | Task | Output |
|---|---|---|
| 1 | Define problem, select dataset | This proposal |
| 2 | Clean & preprocess data | Cleaned dataset + notebook |
| 3 | Exploratory Data Analysis | EDA notebook, 5+ charts |
| 4 | Build interactive dashboard | Power BI / Tableau file |
| 5 | Generate insights & recommendations | Insights document |
| 6 | Present findings | Slide deck |

## 6. Success Metrics
- Dashboard clearly answers: *who* is churning, *why*, and *what to do about it*.
- At least 3 recommendations are specific enough to be handed to a retention
  manager as a starting action plan.
- Analysis is reproducible (clean notebooks, documented steps, versioned on GitHub).

## 7. Expected Outcome
A GitHub repository containing a full, reproducible churn analysis: cleaned
data, EDA, a dashboard, and a set of prioritized, data-backed retention
recommendations.
