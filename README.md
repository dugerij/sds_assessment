# Project Title

## Table of Contents

- [About](#about)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](../CONTRIBUTING.md)

## About <a name="about"></a>

This repository contains the deliverables for the assessment, including:

- Three Jupyter notebooks
- A saved XGBoost model checkpoint (`model_xgb.joblib`)
- A feature column list (`feature_columns.pkl`) used during training

## Getting Started <a name="getting-started"></a>

There are no scripts in this project, but you can explore and test the model through the notebooks. If you'd like to install dependencies and run the notebooks locally:

### Prerequisites

Install dependencies from `requirements.txt`:

```bash
pip install -r requirements.txt
```

## Running Locally
Open the credit_risk_modeling_xgboost_explained.ipynb notebook to explore the model and test predictions.

Usage <a name="usage"></a>
The credit_risk_modeling_xgboost_explained.ipynb notebook contains a score_customers function in the penultimate cell that can be used to make predictions on new customer data.

Example Usage

```python
sample_input = {
    "loan_amount": 2500,
    "term": 36,
    "interest_rate": 13.56,
    ...
}

prediction = score_customers(sample_input)
print(prediction)  # Output: 0 or 1
```

Model and feature files are expected at and are included here:
assets/model_xgb.joblib
assets/feature_columns.pkl

These paths can also be customized via the function arguments.