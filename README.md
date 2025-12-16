# Credit-Risk-Scoring-System
This is my end-to-end Machine Learning project for predicting who's a good credit risk. I started with Data Exploration (EDA), built smart features, and trained a Random Forest. I used SHAP to explain exactly why the model makes its decisions.
# 🏦 Credit Risk Scoring System: Explainable Loan Default Prediction

## 🎯 Goal
Develop, evaluate, and interpret an explainable ML model to predict the probability of loan default (risk) using the German Credit Dataset.

## 🚀 Key Results

The final **Random Forest Classifier** model achieved strong performance on the imbalanced dataset:

| Metric | Score | Priority |
| :--- | :--- | :--- |
| **ROC-AUC** | **~0.76** | Discrimination Power |
| **Recall** | **~85%** | Capturing True Defaulters |

## 🧠 Core Insights (Model Interpretation via SHAP)

SHAP analysis ensured model transparency and identified the true risk drivers: 

1.  **Checking Account Status:** The **most influential factor**, highly predictive of risk if overdrawn or non-existent.
2.  **Duration in Months:** Longer loan terms significantly increase default probability.
3.  **Credit History:** Primary indicator of risk, driving decisions toward approval or rejection.

## 🛠️ Project Contents

* `Credit_Risk_Scoring.ipynb`: Complete E2E pipeline (EDA, Feature Engineering, LogReg, Random Forest, SHAP).
* `requirements.txt`: Python dependencies for reproducibility.

## 💡 Next Step
The project is ready for the **Deployment Phase**, including creating a scoring API (FastAPI) and a user interface (Streamlit).

The analytical phase is complete. The next step is to transition the model into a production environment:

1.  **Deployment:** Expose the trained risk-scoring logic via a fast **FastAPI** web service.
2.  **Front-End:** Build a quick, interactive interface using **Streamlit** to allow loan officers to input data and receive real-time risk scores.

