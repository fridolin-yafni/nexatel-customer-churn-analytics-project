# NexaTel Customer Churn Analytics Project

End-to-end customer churn analytics project for a telecom company (NexaTel) — covering data cleaning, exploratory data analysis, churn KPI calculations, and a 5-page Power BI dashboard with an executive summary report.

## Project Overview

This project analyzes customer churn for NexaTel, a telecom provider, using customer, subscription, support ticket, contract, and campaign data. The goal was to identify why customers churn, quantify its business impact, and present actionable insights to leadership through a dashboard and a management report.

## Tools Used

- **Python (pandas)** — data cleaning, KPI calculations, cohort retention analysis
- **Jupyter Notebook** — all analysis and calculations
- **Power BI** — interactive 5-page dashboard with DAX measures
- **Microsoft Word** — management summary report

## Project Phases

**Phase 1 — Data Cleaning**
Cleaned raw customer, subscription, support ticket, and contract datasets. Fixed mixed date formats (DD-MM-YYYY and YYYY/MM/DD), handled missing/invalid values, and removed personally identifiable information (PII) before analysis.

**Phase 2 — Exploratory Data Analysis**
Explored churn patterns across customer segments, tenure bands, billing cycles, complaints, network quality, and regions to surface early trends.

**Phase 3 — Churn KPI Calculations**
Calculated core business KPIs for the Feb 2026 period:
- Customer Churn Rate: 0.91%
- Retention Rate: 99.09%
- Monthly Recurring Revenue (MRR): ₹15,087,084
- ARPU: ₹960.07
- Customer Lifetime Value (CLV): ₹63,409
- Revenue Lost to Churn: ₹90,782
- First Contact Resolution (FCR): 42.25%
- Avg Resolution Time: 15.4 hours
- Contract Renewal Rate: 65.79%
- Avg Customer Tenure: 86.2 months

Also built a bonus 3/6/12-month cohort retention analysis to track how different acquisition cohorts retain over time.

**Phase 4 — Power BI Dashboard & Management Report**
Built a 5-page interactive dashboard:
1. **Executive Overview** — headline KPIs and churn trend
2. **Customer & Segment** — churn by segment, tenure, ARPU distribution, at-risk customers
3. **Service & Support** — FCR, resolution time, churn vs. complaint resolution status
4. **Network & Regional** — churn by state, network quality map, dropped-call rate vs. churn correlation
5. **Campaigns & Revenue** — retention campaign outcomes, MRR and revenue-lost trends

Paired with a 2-page Management Summary Report for the Chief Customer Officer, covering key findings, risks, opportunities, and recommendations.

## Key Findings

- Monthly churn rate held steady around **0.9%**, but customers with unresolved complaints churn at **25.6%** vs. **15.1%** for those without — complaint resolution is a strong churn driver.
- First Contact Resolution is low at **42%**, well below the healthy benchmark (~78%+), pointing to a support-quality gap.
- Cities with dropped-call rates above **~2.8%** show visibly higher churn, suggesting network quality contributes to customer loss alongside support issues.
- Contract renewal rate is **65.8%**, leaving meaningful room for improvement through retention campaigns, which currently show an **86.8%** acceptance-to-retention rate when used.

## Files in This Repository

| File | Description |
|---|---|
| `Phase1_DataCleaning_FridolinYafni_P.ipynb` | Data cleaning notebook |
| `Phase2_EDA_FridolinYafni_P.ipynb` | Exploratory data analysis notebook |
| `Phase3_KPIs_FridolinYafni_P.ipynb` | Churn KPI calculations + cohort retention |
| `Phase4_Dashboard_FridolinYafni_P.pbix` | Power BI dashboard (5 pages) |
| `Phase4_Report_FridolinYafni_P.docx` | Management summary report |
