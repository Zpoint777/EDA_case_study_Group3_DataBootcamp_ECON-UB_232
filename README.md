# EDA_case_study_Group3_DataBootcamp_ECON-UB_232

# Exploratory Data Analysis (EDA): Loan Default Risk

## Project Overview
This project conducts an **Exploratory Data Analysis (EDA)** on loan application data to understand the key factors associated with **loan default risk**.  
The analysis is motivated by a common challenge in consumer finance: making accurate lending decisions when applicants have limited or imperfect credit histories.

By examining both **current applicant characteristics** and **historical loan behavior**, this study aims to identify patterns that distinguish **likely defaulters** from **non-defaulters**, supporting more informed credit risk assessment and decision-making.

---

## Business Objective
The primary objectives of this analysis are to:

- Identify key variables that are strongly associated with loan default
- Understand how applicant financial attributes influence repayment behavior
- Examine how historical loan outcomes and borrowing behavior affect default risk
- Provide insights that can support business actions such as loan approval decisions, interest rate adjustments, and risk-based pricing

The ultimate goal is to **reduce default risk while avoiding unnecessary rejection of creditworthy applicants**.

---

## Data Description
The analysis uses three datasets:

- **application_data.csv**: Information on current loan applicants, including demographic and financial attributes, as well as the target variable indicating default status.
- **previous_application.csv**: Historical loan application records for the same clients, including loan terms, approval outcomes, interest rate groups, and repayment-related variables.
- **columns_description.xlsx**: A data dictionary describing the meaning of each variable.

---

## Analysis Summary
The EDA focuses on understanding how both **current application features** and **historical loan behavior** relate to default probability.  
Key techniques include data grouping, binning continuous variables, computing default rates, and visualizing patterns using bar charts.

The overall default rate in the dataset is approximately **8%**, indicating a highly imbalanced classification problem typical in credit risk analysis.

---

## Key Findings
The most important indicators associated with higher default risk identified in this analysis include:

- **Low external credit score (EXT_SOURCE_3)**: Strong monotonic relationship with default probability.
- **Low down payment ratio**: Higher upfront contribution is associated with lower default risk.
- **High interest rate group (NAME_YIELD_GROUP)**: Reflects risk-based pricing and higher default likelihood.
- **Long previous loan terms (CNT_PAYMENT)**: Longer repayment periods are linked to higher default rates.
- **Recent borrowing activity (DAYS_DECISION)**: More recent loans are associated with increased default risk.
- **Multiple previously refused applications**: Indicates historical creditworthiness issues.
- **High borrowing frequency**: A larger number of previous loans corresponds to higher default risk.
- **Zero down payment history**: Suggests higher leverage and increased credit risk.

Historical behavioral variables demonstrate strong explanatory power and complement current applicant information.

---

## Repository Structure
The repository is organized as follows:

- `EDA_Loan_Default_Analysis.ipynb` – Jupyter Notebook containing the full exploratory data analysis, visualizations, and interpretations
- `slides/` – A brief slide presentation summarizing the key findings
- `README.md` – Project overview, objectives, data description, and key insights

---

## Conclusion
This exploratory analysis demonstrates that both **applicant characteristics** and **historical loan behavior** play a significant role in determining loan default risk.

External credit score and down payment ratio emerge as the strongest predictors, while behavioral variables such as refusal history, loan frequency, interest rate level, and borrowing recency provide additional valuable signals.

These findings highlight the importance of incorporating both current financial information and past behavioral patterns into credit risk assessment and lending strategy development.
