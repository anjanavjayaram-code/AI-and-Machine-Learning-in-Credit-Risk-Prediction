Data Sources Documentation
Overview

This project uses a publicly available consumer credit dataset derived from LendingClub loan data to evaluate and compare traditional statistical models and machine learning techniques for credit risk prediction.

The dataset is used exclusively for academic and research purposes and supports transparency, reproducibility, and ethical compliance.

Dataset Description

Dataset name: LendingClub Consumer Loan Dataset

Observational unit: Individual consumer loan

Target variable: Loan default (binary outcome)

Sample size: 5,000 loan observations (subset used for analysis)

Data type: Structured tabular data

Each record represents a borrower’s loan application and repayment outcome, including financial, credit history, and loan-specific attributes.

Data Source and Origin

The dataset is sourced from LendingClub, a US-based peer-to-peer lending platform, and is commonly used in academic research and data science benchmarking studies.

Original source: LendingClub public loan data

Distribution platform: Kaggle (public data repository)

Access type: Open-access, publicly available

The dataset has been widely used in peer-reviewed studies examining credit risk modelling and machine learning performance in consumer lending contexts.

Nature of the Data

The data is real-world historical loan data, not simulated.

All borrower information has been anonymised prior to public release.

No personally identifiable information (PII) is included.

The dataset contains no direct protected attributes (e.g. race, religion).

Key Variables Used

The analysis uses a subset of variables commonly applied in credit risk modelling, including:

Loan characteristics (e.g. loan amount, term, interest rate)

Borrower financial attributes (e.g. income, debt-to-income ratio)

Credit history indicators (e.g. FICO score, delinquencies)

Loan outcome status (used to derive default label)

A full variable description and preprocessing rationale are documented in the project notebook.

Default Definition

Default is defined in line with industry practice:

Loans with status “Charged Off” or “Default” are classified as default events.

Loans marked “Fully Paid” are classified as non-default.

This binary classification aligns with probability-of-default (PD) modelling conventions used in consumer credit risk analysis.

Licensing and Usage Rights

The dataset is distributed under Kaggle’s data usage terms.

Use is permitted for educational and research purposes.

The dataset is not redistributed or modified for commercial use within this project.

Users intending to reuse the data should consult the original Kaggle dataset page for the most up-to-date licensing conditions.

Ethical Considerations

Ethical considerations have been explicitly addressed:

All data are publicly available and anonymised

No automated credit decisions are made based on this analysis

The project complies with principles of responsible data use, transparency, and accountability

Results are interpreted cautiously to avoid misleading or discriminatory conclusions

The dataset does not contain explicit demographic variables, which limits fairness analysis but also reduces the risk of direct discriminatory modelling.

Reproducibility

The dataset is stored locally in the data/ directory to ensure:

Full reproducibility of results

Consistency between reported findings and underlying data

Transparency for academic review and validation

All preprocessing, feature selection, and modelling steps are documented in the accompanying Jupyter Notebook.

Disclaimer

This dataset and analysis are used solely for academic research.
The results are not intended for real-world credit decision-making without further validation, governance controls, and regulatory approval.
