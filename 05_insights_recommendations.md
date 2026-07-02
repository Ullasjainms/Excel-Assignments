# Insights & Recommendations: Reducing Customer Churn

## Recap of the Business Problem
> "The company is losing approximately 1 in 4 customers to churn. Which customer
> segments are most likely to churn, and what specific, actionable steps can the
> retention team take to reduce churn rate?"

Overall churn rate across the customer base: **22.3%** (1,571 of 7,043 customers).

---

## Insight 1: Contract length is the single biggest churn driver
- Month-to-month customers churn at **31.4%**
- One-year contract customers churn at **13.1%**
- Two-year contract customers churn at **10.2%**

Month-to-month customers churn at roughly **3x** the rate of two-year customers, and they make up more than half of the customer base — this is the largest, highest-leverage segment in the dataset.

**Recommendation:** Launch a contract-conversion campaign targeting month-to-month customers, offering a modest discount (e.g., 10% off) or a value-add (e.g., free premium tech support for 3 months) in exchange for switching to a one-year contract. Prioritize customers in months 3–9 of tenure, before they've decided to leave but after they've had time to evaluate the service.

---

## Insight 2: The first year of the relationship is the highest-risk window
- 0–12 months tenure: **29.0%** churn
- 13–24 months: **19.4%** churn
- 25–48 months: **17.2%** churn
- 49+ months: **15.9%** churn

Churn risk drops steadily the longer a customer stays, meaning the first year is disproportionately important to get right.

**Recommendation:** Build a structured onboarding and check-in program for new customers: a welcome call in week 1, a proactive check-in at day 30, and a satisfaction survey at day 90 with an offer to resolve any issues before they consider leaving. Even a small reduction in first-year churn compounds over the customer's full lifetime.

---

## Insight 3: Fiber optic customers churn more than DSL customers
- Fiber optic: **27.9%** churn
- DSL: **18.6%** churn
- No internet service: **16.7%** churn

Fiber optic is the company's premium (higher-priced) internet product, yet it has the highest churn rate of any internet service type. This suggests either a pricing/value mismatch or service reliability issues specific to fiber.

**Recommendation:** Investigate fiber-specific service complaints and support tickets, and review fiber pricing relative to competitors in the same markets. Consider a loyalty discount tier for long-tenured fiber customers to protect this higher-revenue segment.

---

## Insight 4: Manual payment methods correlate with higher churn
- Electronic check: **28.1%** churn
- Mailed check: **19.8%** churn
- Bank transfer (automatic): **19.5%** churn
- Credit card (automatic): **18.9%** churn

Customers on manual payment methods — especially electronic check — churn noticeably more than customers on autopay. This may reflect lower overall engagement/convenience adoption rather than payment method itself, but it's a strong, easy-to-target signal.

**Recommendation:** Run a targeted campaign encouraging electronic-check customers to switch to autopay (credit card or bank transfer), using a small one-time bill credit as an incentive. Autopay reduces friction and is also operationally cheaper to process.

---

## Revenue Impact
Using the dashboard's "Monthly revenue at risk" metric (sum of `MonthlyCharges` for currently churned customers), churned customers represent a significant share of monthly recurring revenue. Even a **5-percentage-point reduction** in overall churn (from 22.3% to ~17.3%) would retain roughly **350 additional customers** and their associated monthly revenue — see the dashboard for the live, filterable revenue-at-risk figure by segment.

---

## Summary of Recommendations, Prioritized

| Priority | Recommendation | Target segment | Expected effect |
|---|---|---|---|
| 1 | Contract-conversion incentive | Month-to-month customers | Largest volume, largest churn gap |
| 2 | First-year onboarding & check-in program | 0–12 month tenure customers | Reduces the highest-risk window |
| 3 | Autopay adoption campaign | Electronic check payers | Low-cost, high-response segment |
| 4 | Fiber service/pricing review | Fiber optic customers | Protects premium revenue segment |

## Next Steps
- Pilot the contract-conversion and autopay campaigns on a small segment first, measure churn rate change over one quarter before rolling out company-wide.
- Build a predictive churn model (logistic regression or gradient boosting) using these same features to score customers by churn risk in real time, so retention teams can act proactively rather than reactively.
- Re-run this analysis quarterly to track whether the interventions are moving the churn rate.
