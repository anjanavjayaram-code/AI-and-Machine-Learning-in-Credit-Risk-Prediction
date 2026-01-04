# Data Sources Documentation

## Overview

This project uses a **single publicly available dataset** for consumer credit risk modelling.  
The dataset contains anonymised borrower-level and loan-level information and is widely used in academic research and applied machine learning studies on credit risk prediction.

All data used in this project are **secondary, anonymised, and publicly accessible**, ensuring transparency, reproducibility, and compliance with ethical research standards.

---

## Primary Dataset

### LendingClub Consumer Loan Dataset

- **Source**: LendingClub (via Kaggle)
- **Access Link**:  
  https://www.kaggle.com/datasets/wordsforthewise/lending-club
- **Data Type**: Structured tabular data
- **File Used**: `lendingclub.csv`
- **Observations**: 5,000 loans
- **Variables**: 11 original variables + 1 derived target variable
- **Time Coverage**: Multiple loan origination years (as provided in the public dataset)
- **Geographical Scope**: United States consumer lending market

LendingClub is a peer-to-peer lending platform that publicly releases anonymised loan-level data for research and transparency purposes. The dataset includes borrower financial characteristics, loan attributes, and repayment outcomes.

---

## Target Variable Construction

The original dataset contains a categorical loan status variable:

- `loan_status`

For the purpose of credit risk modelling, a **binary default indicator** was constructed:

- Loans labelled as **“Charged Off”** or **“Default”** were classified as **default events (1)**
- Loans labelled as **“Fully Paid”** were classified as **non-default events (0)**

This transformation is consistent with industry-standard probability-of-default (PD) modelling practices and prior academic research.

---

## Variables Used in the Analysis

The project uses a subset of economically meaningful variables commonly applied in consumer credit risk modelling:

### Loan Characteristics
- `loan_amnt` – Loan amount issued
- `term` – Loan term (36 or 60 months)
- `int_rate` – Interest rate applied to the loan

### Borrower Financial Information
- `annual_inc` – Annual income
- `dti` – Debt-to-income ratio
- `emp_length` – Employment length

### Credit History Indicators
- `fico_score` – Borrower credit score
- `open_acc` – Number of open credit accounts
- `credit_utilization` – Credit utilisation ratio
- `delinq_2yrs` – Number of delinquencies in the past two years

These variables were selected based on:
- Prior academic literature
- Industry credit scoring practices
- Economic interpretability and regulatory relevance

---

## Data Quality and Preprocessing

- The dataset used in this project contains **no missing values** in the selected variables.
- Numerical variables were standardised using **z-score normalisation**.
- Categorical variables (`term`, `emp_length`) were encoded using **one-hot encoding**.
- No synthetic data generation or external data enrichment was applied.
- The original class imbalance in default outcomes was preserved to reflect real-world credit portfolios.

---

## Ethical and Legal Considerations

- All data are **fully anonymised** and contain **no personally identifiable information (PII)**.
- The dataset is publicly available and intended for research and educational use.
- The project complies with data protection principles and aligns with GDPR requirements regarding transparency and accountability in automated decision-making.
- No protected attributes (e.g., race, gender, religion) are included in the dataset.

---

## Limitations of the Data

- The dataset represents a **public, simplified subset** of LendingClub loan data and may not fully reflect proprietary banking datasets.
- The absence of explicit demographic variables limits the scope of fairness and bias assessment.
- The data reflect historical lending conditions and may not capture real-time or dynamic borrower behaviour.

These limitations are acknowledged and considered in the interpretation of analytical results.

---

## Reproducibility

All data preprocessing, feature engineering, and modelling steps are fully documented in the project’s Jupyter Notebooks.  
Using the provided dataset and code, the analysis can be independently replicated.

---

## Citation

If using this dataset or reproducing the analysis, please cite:

LendingClub (via Kaggle). *LendingClub Loan Dataset*.  
https://www.kaggle.com/datasets/wordsforthewise/lending-club
