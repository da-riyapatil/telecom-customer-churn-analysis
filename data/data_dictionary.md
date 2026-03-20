# Data Dictionary

## Dataset Overview
This project uses a telecom customer dataset with **7,043 records** and **23 columns**.

The dataset contains customer demographic details, service usage, billing information, support-related fields, and churn status.

> **Note:** `TotalCharges` contained some blank values and required cleaning before analysis.

---

## Column Dictionary

| Column Name | Data Type | Description |
|---|---|---|
| customerID | Text | Unique ID for each customer |
| gender | Text | Customer gender |
| SeniorCitizen | Numeric / Binary | Whether the customer is a senior citizen (0 = No, 1 = Yes) |
| Partner | Text | Whether the customer has a partner |
| Dependents | Text | Whether the customer has dependents |
| tenure | Numeric | Number of months the customer has stayed with the company |
| PhoneService | Text | Whether the customer has phone service |
| MultipleLines | Text | Whether the customer has multiple phone lines |
| InternetService | Text | Type of internet service used by the customer |
| OnlineSecurity | Text | Whether the customer has online security service |
| OnlineBackup | Text | Whether the customer has online backup service |
| DeviceProtection | Text | Whether the customer has device protection service |
| TechSupport | Text | Whether the customer has tech support service |
| StreamingTV | Text | Whether the customer uses streaming TV service |
| StreamingMovies | Text | Whether the customer uses streaming movies service |
| Contract | Text | Customer contract type |
| PaperlessBilling | Text | Whether the customer uses paperless billing |
| PaymentMethod | Text | Customer payment method |
| MonthlyCharges | Decimal | Monthly amount charged to the customer |
| TotalCharges | Decimal | Total amount charged to the customer over the full tenure |
| numAdminTickets | Numeric | Number of administrative support tickets raised by the customer |
| numTechTickets | Numeric | Number of technical support tickets raised by the customer |
| Churn | Text | Whether the customer left the company |

---

## Important Columns for Analysis

| Column Name | Why It Matters |
|---|---|
| Churn | Target variable used to identify whether a customer left |
| Contract | Helps compare churn across contract types |
| InternetService | Helps analyze churn by service type |
| PaymentMethod | Helps identify billing-related churn patterns |
| tenure | Used to study churn by customer duration |
| MonthlyCharges | Helps compare cost and churn behavior |
| TechSupport | Useful for understanding retention vs support service usage |
| OnlineSecurity | Useful for comparing churn across support-related services |
| numTechTickets | Helps identify whether technical issues are linked to churn |

---

## Derived Fields Used in Power BI

| Field Name | Description |
|---|---|
| Total Customers | DAX measure for total customer count |
| Churn Rate | DAX measure for churn percentage |
| Churned Customers | DAX measure for customers with churn = Yes |
| Monthly Revenue | Sum of monthly charges |
| Total Revenue | Sum of total charges |
| Tenure in Years | Derived field created from monthly tenure |
| Customer Segmentation / Tenure Groups | Grouped fields used for dashboard analysis |

---

## Value Examples

- **Contract:** Month-to-month, One year, Two year
- **InternetService:** DSL, Fiber optic, No
- **PaymentMethod:** Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic)
- **Churn:** Yes, No