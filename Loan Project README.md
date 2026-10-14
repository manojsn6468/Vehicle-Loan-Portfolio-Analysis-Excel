# L\&T Vehicle Loan Portfolio \& Branch Performance Analytics

## Project Overview

This project analyzes **233,154 vehicle-loan records** using **Microsoft Excel, Power Query, PivotTables, PivotCharts, and Slicers**. The objective is to understand portfolio performance, disbursement trends, customer/loan risk, default behavior, and branch-level risk.

The project contains two interactive Excel dashboards:

1. **Loan Portfolio and Branch Performance**
2. **Vehicle Loan Default \& Risk Analysis**

## Tools Used

* Microsoft Excel
* Power Query
* PivotTables
* PivotCharts
* Slicers

## Data Preparation

* Renamed all **41 original source columns** into business-friendly names.
* Replaced missing **Employment Type** values with `Unknown` rather than deleting records or assuming a category.
* Corrected one obvious future-date DOB data-quality issue from `15/09/2049` to `15/09/1949`.
* Created **Customer Age** from Disbursal Date and Date of Birth.
* Created analysis groups for:

  * Age Group
  * LTV Group
  * Loan Amount Group
* Created **Loan Default Status** where `1 = Default` and `0 = No Default`.
* Created **Disbursal Month, Disbursal Week, and Disbursal Month No.** for trend analysis and sorting.

## Key KPIs

|KPI|Value|
|-|-:|
|Total Loans|233,154|
|Total Disbursed Amount|₹1,267.36 Cr|
|Average Loan Amount|₹54,357|
|Average Asset Cost|₹75,865|
|Average LTV|74.75%|
|Defaulted Loans|50,611|
|Default Rate|21.71%|

## Dashboard 1 - Loan Portfolio and Branch Performance

### KPIs

* Total Loans
* Total Disbursed Amount
* Average Loan Amount
* Average Asset Cost
* Average LTV
* Defaulted Loans
* Default Rate %

### Charts

* Weekly Disbursement Trend
* Top 10 Branches by Disbursed Amount
* Top 10 States by Disbursed Amount
* Manufacturer-wise Disbursement
* Loans by Employment Type

### Slicers

* Disbursal Month
* Branch ID
* State ID
* Manufacturer ID
* Employment Type
* LTV Group

## Dashboard 2 - Vehicle Loan Default \& Risk Analysis

**Focus:** Customer Risk | Loan Risk | Branch Risk

### KPIs

* Total Loans
* Defaulted Loans
* Default Rate %
* Average LTV

### Charts

* Default Rate by Age Group
* Default Rate by LTV Group
* Default Rate by Loan Amount Group
* Default Rate by Employment Type
* Top 10 Branches by Default Rate

### Slicers

* Disbursal Month
* Branch ID
* State ID
* Employment Type
* LTV Group
* Loan Amount Group

## Key Insights

* Overall default rate is **21.71%** with **50,611** defaulted loans.
* The **18-25** age group has the highest age-band default rate at approximately **23.88%**.
* The **80-89% LTV** group shows the highest default rate among LTV bands at approximately **25.88%**.
* The **75K-99K** loan amount group shows the highest default rate among loan-size groups at approximately **26.08%**.
* **Self employed** customers have a higher default rate (\~**22.77%**) than **Salaried** customers (\~**20.35%**).
* **Branch 251** has the highest default rate in the Top 10 branch-risk view at approximately **34.39%**.

## Repository Files

Recommended repository structure:

```text
L\\\\\\\&T-Vehicle-Loan-Analytics/
├── README.md
├── images/
│   ├── dashboard-1-portfolio.png
│   └── dashboard-2-risk.png
├── docs/
│   └── LT\\\\\\\_Vehicle\\\\\\\_Loan\\\\\\\_Project\\\\\\\_Notes\\\\\\\_Updated.docx
└── workbook/
    └── vehicle-loan-analytics.xlsx   (Git LFS or cloud link recommended)
```

> The final workbook is large (about 89 MB). For a clean portfolio repository, keep dashboard screenshots and documentation directly in GitHub and use Git LFS or a cloud link for the full workbook if needed.

## Project Outcome

The project demonstrates practical Excel data-analysis skills across **data cleaning, Power Query transformation, KPI design, PivotTable analysis, interactive dashboarding, risk segmentation, and business insight genera**

