# Customer Churn Prediction

## Overview
An end-to-end Machine Learning project that predicts whether a telecom customer is likely to leave the service. The project explores customer data, preprocesses numerical and categorical features, trains classification models, and evaluates their performance.

## Problem Statement
Customer churn affects customer retention and business revenue. The goal of this project is to identify customers who may be likely to churn so that telecom companies can investigate risks and develop targeted retention strategies.

## Dataset
This project uses the Telco Customer Churn dataset for educational and portfolio purposes.
The dataset is not included in this repository. Please obtain it from the original source and review the applicable licence and usage terms before downloading or redistributing it.
The notebook expects the CSV file at data/Churn-Dataset.csv.

- Target variable: `Churn`
- `No` is encoded as `0`, and `Yes` as `1`
- The dataset contains customer demographics, account details, services, contract information, and billing details.

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Git and GitHub

## Project Workflow
1. Data loading and exploratory data analysis (EDA)
2. Data cleaning and missing-value handling
3. Train-test splitting with stratification
4. Numerical preprocessing using median imputation and standardization
5. Categorical preprocessing using most-frequent imputation and one-hot encoding
6. Model training and comparison
7. Evaluation using accuracy, precision, recall, F1-score, and ROC-AUC
8. Classification-threshold analysis
9. Interpretation of Logistic Regression coefficients

## Models
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

## Evaluation
The Logistic Regression model achieved a ROC-AUC score of **0.8419** on the test set.

ROC-AUC evaluates how well the model ranks churners above non-churners across different classification thresholds. Additional classification metrics are used to assess the trade-off between detecting churners and avoiding false alarms.

## Business Insights
- Customers with shorter tenure may need additional onboarding and retention support.
- Customers on month-to-month contracts may be candidates for retention campaigns.
- Fiber-optic customers warrant further investigation into pricing, service quality, and customer satisfaction.
- Churn predictions can help prioritize customer outreach and retention efforts.

These findings represent associations learned from historical data and do not establish causation.

## Limitations
- Model performance depends on the quality and representativeness of the dataset.
- The classification threshold affects precision and recall.
- Model associations do not prove that a customer characteristic causes churn.
- Retention strategies should be tested before assuming they will reduce churn.

## How to Run
1. Clone the repository.
2. Create and activate a Python virtual environment.
3. Install the dependencies.
4. Place the dataset in the expected `data/` directory, it is not included in the repository.
5. Open the notebook in Jupyter or VS Code and run the cells in order.

Install dependencies:

```bash
pip install -r requirements.txt
```

## Future Improvements
- Evaluate feature importance using permutation importance.
- Tune models and classification thresholds using validation data or cross-validation.
- Build a simple prediction interface using Streamlit.

## Author
**Anwesh A Salian**

GitHub: [Anwesh-A-Salian](https://github.com/Anwesh-A-Salian)