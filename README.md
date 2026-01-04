AI and Machine Learning in Credit Risk Prediction
Project Overview

This project evaluates whether artificial intelligence (AI) and machine learning (ML) techniques can improve consumer credit risk prediction compared to traditional statistical models, while remaining suitable for use in regulated financial environments.

Credit risk prediction is a core function in financial institutions, directly influencing lending decisions, capital adequacy, regulatory compliance, and long-term financial performance. Traditional approaches such as logistic regression are widely used due to their interpretability and regulatory acceptance, but may struggle to capture nonlinear relationships and complex interactions present in modern, data-rich lending environments.

This repository supports an academic project that compares traditional statistical models and advanced machine learning models using a publicly available consumer credit dataset. The emphasis is not only on predictive performance, but also on interpretability, governance, and responsible AI deployment.

Research Objectives

The project addresses the following objectives:

To compare traditional statistical credit risk models with modern machine learning techniques

To evaluate predictive performance using industry-standard metrics for imbalanced classification

To assess the suitability of machine learning models for regulated financial decision-making

To examine model interpretability using feature importance and risk-theoretic alignment

To explore fairness and governance considerations in AI-driven credit scoring

Gradient boosting is used primarily as a risk ranking and probability estimation tool rather than a standalone binary decision system, with final lending decisions assumed to involve human oversight and governance controls.

Methods and Models

The analysis follows a quantitative, comparative modelling framework using Python and scikit-learn.

Models Evaluated

Logistic Regression (baseline statistical model)

Decision Tree

Random Forest

Gradient Boosting (primary ensemble model)

Evaluation Metrics

AUC-ROC (primary metric for risk ranking)

Accuracy

Precision

Recall

F1-score

Confusion matrix analysis

Given the presence of class imbalance, model performance is interpreted cautiously, with a focus on ranking quality rather than raw classification accuracy.

Repository Structure
AI-and-Machine-Learning-in-Credit-Risk-Prediction/
│
├── README.md
├── data/
│   ├── lendingclub.csv
│   └── README_data_sources.md
│
├── notebooks/
│   └── credit_risk_analysis.ipynb
│
├── results/
│   └── figures/
│
└── requirements.txt
Data Sources

The project uses a publicly available LendingClub consumer loan dataset.

The dataset contains anonymised borrower-level information and loan outcomes.

Default is defined based on loan status (e.g. Charged Off).

The dataset is used strictly for academic and research purposes.

Full details regarding data origin, licensing, variables, and preprocessing decisions are provided in:
data/README_data_sources.md
What the Notebook Contains

The main notebook includes:

Data loading and preprocessing

Feature engineering aligned with credit risk theory

Model training and evaluation

ROC curve comparison across models

Confusion matrix analysis

Global feature importance analysis

Predicted probability (PD) analysis

Socioeconomic subgroup comparison (income groups)

Interpretation of results from a regulatory and business perspective

Ethical and Regulatory Considerations

All data used are public and anonymised

No automated decisions are assumed without human oversight

Model interpretability is prioritised over black-box optimisation

The project aligns with principles from GDPR and financial model governance frameworks

Intended Use

This repository supports an academic MSc project in data analytics / financial analytics.
It is not intended for production deployment without additional validation, governance, and regulatory approval.

Author
MSc Project – AI and Machine Learning in Credit Risk Prediction
