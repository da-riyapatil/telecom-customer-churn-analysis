# Telecom Customer Churn Analysis Dashboard
![PowerBI customer churn dashboard](<screenshots/power bi dashboard.png>)

## Project Links
- **Power BI Dashboard:** [View Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiOWUyZjJlNTMtNjYxNC00Y2VjLWI2YTYtYmYzNzQ0ODdlOTMxIiwidCI6IjI1Y2UwMjYxLWJiZDYtNDljZC1hMWUyLTU0MjYwODg2ZDE1OSJ9)

## Summary
This project is a **Forage internship-style telecom churn analysis project** based on a provided dataset and business problem.

The work focused on:
- cleaning and preparing customer data
- creating DAX measures and calculated columns
- building an interactive Power BI dashboard
- identifying churn patterns and customer risk segments

## Business Problem
Telecom companies lose revenue when customers leave their services.  
This project analyzes customer churn to understand which groups are more likely to leave and what factors are linked with higher churn.

It helps answer questions such as:
- Which contract types have the highest churn?
- Which payment methods are linked with churn?
- Does internet service type affect churn?
- Are support services helping retention?
- Are newer customers leaving earlier?

## Tools & Technologies
- **Power BI**
- **DAX**
- **Power Query**
- Data cleaning and preparation
- Dashboard design and KPI reporting

## Key Insights
- Month-to-month customers had the highest churn rate at 42.71% vs 11.27% for one-year and 2.83% for two-year contracts
- Fiber optic customers showed 41.89% churn, higher than DSL at 18.96% and no internet service at 7.40%
- Electronic check users had the highest churn rate at 45.29%, while automatic payment methods were lower at 15% to 17%
- Customers without support services churned far more, including 41.77% without Online Security and 41.64% without Tech Support
- Customers in their first 0 to 12 months had 47.44% churn vs 17.13% for customers with longer tenure
- A high-risk segment (month-to-month + electronic check + fiber optic) showed about 60.37% churn across 1,307 customers

## Business Recommendations
- Target month-to-month customers with retention offers and contract upgrades
- Improve service experience for fiber users to reduce churn in that segment
- Encourage automatic payment methods to lower churn risk
- Promote support services to improve customer retention
- Focus on early-stage customer engagement to reduce first-year churn

## Repository Structure
```text
telecom-customer-churn-analysis/
│
├── powerbi/
│   └── churn_dashboard.pbix
│
├── docs/
│   ├── project_summary.md
│   ├── insights_and_recommendations.md
│   ├── powerbi_service_features.md
│
├── data/
│   └── data_dictionary.md
│
├── screenshots/
│   └── (dashboard images)
│
├── README.md
└── .gitignore
```

## How to View Project

- Open the Power BI dashboard link above for the interactive version
- Open powerbi/churn_dashboard.pbix in Power BI Desktop to review the report
- Check the screenshots/ folder for dashboard images
- Read the files in docs/ for project summary, insights, and Power BI Service notes