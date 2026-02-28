# EDA_case_study_Group3_DataBootcamp_ECON-UB_232

# Exploratory Data Analysis (EDA): Loan Default Risk

## Project Overview
This project conducts an Exploratory Data Analysis (EDA）on loan application data to understand the key factors associated with loan default risk.  
The analysis is motivated by a common challenge in consumer finance: making accurate lending decisions when applicants have limited or imperfect credit histories.

By examining both current applicant characteristics and historical loan behavior, this study aims to identify patterns that distinguish likely defaulters from non-defaulters, supporting more informed credit risk assessment and decision-making.

---

## Business Objective
The primary objectives of this analysis are to:

- Identify key variables that are strongly associated with loan default
- Understand how applicant financial attributes influence repayment behavior
- Examine how historical loan outcomes and borrowing behavior affect default risk
- Provide insights that can support business actions such as loan approval decisions, interest rate adjustments, and risk-based pricing

The ultimate goal is to reduce default risk while avoiding unnecessary rejection of creditworthy applicants.

---

## Data Description
The analysis uses three datasets:

- application_data.csv: Information on current loan applicants, including demographic and financial attributes, as well as the target variable indicating default status.
- previous_application.csv: Historical loan application records for the same clients, including loan terms, approval outcomes, interest rate groups, and repayment-related variables.
- columns_description.xlsx: A data dictionary describing the meaning of each variable.

---

## Analysis Summary
The EDA focuses on understanding how both current application features and historical loan behavior relate to default probability.  
Key techniques include data grouping, binning continuous variables, computing default rates, and visualizing patterns using bar charts.

The overall default rate in the dataset is approximately 8%, indicating a highly imbalanced classification problem typical in credit risk analysis.

---

## Key Findings
The following factors were identified as the strongest predictors of increased risk:

1. External & Financial Indicators

External Credit Scores (EXT_SOURCE_2/3): The strongest predictors identified. Applicants with low scores have a 11.2% default rate, compared to just 4.9% for high-scoring applicants.

Income Type: "Working" individuals show a 9.6% default rate, significantly higher than "Pensioners" at 5.4%.

2. Demographic & Stability Factors

Education Level: Risk decreases as education increases. Lower secondary education carries a 10.9% risk, while Academic degrees drop to a mere 1.8%.

Housing Type: Applicants in rented apartments or living with parents are high-risk (over 12% default rate), while those in office or co-op apartments are much more stable (6.5% – 8.5%).

Family Status: Single individuals and those in civil marriages approach a 10% default rate. Widows represent the lowest risk group at 6%.

3. Contractual & Behavioral Risks

Contract Type: Cash loans (8.3%) are significantly riskier than Revolving loans (5.5%).
City Registration Mismatch: A 49% increase in default risk (from 7.3% to 10.6%) was observed when an applicant's registered city did not match their work city.

Loan History: Longer previous terms, zero down payments, and high frequencies of previous refusals all correlate with higher current risk.

---

## Repository Structure
The repository is organized as follows:

- `EDA__activity_historyloadn_Zien.ipynb` – Jupyter Notebook containing selected visualizations and interpretations
- `Ishaan_Banerjee_EDA_activity.ipynb` – Selected points of analysis
- `Jasmine.ipynb` – Selected points of analysis
- `EDA_Findings.pdf` – Detailed slide presentation of categorical and numerical findings.
- `README.md` – Project overview, objectives, data description, and key insights

---

## Conclusion
The analysis demonstrates that default risk is not driven by a single factor but by a combination of financial score and social stability. High-risk profiles are characterized by lower education levels, non-ownership housing, and informal family structures.

Strategically, the data suggests that lenders can significantly mitigate risk by prioritizing applicants with higher educational attainment and more stable housing/marital status, even when traditional credit scores are intermediate.
