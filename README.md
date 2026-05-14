# Stroke Prediction Using Machine Learning

## Project Overview

This project applies machine learning techniques to predict the occurrence of stroke using demographic and clinical health data. The workflow includes data preprocessing, missing-value imputation, class-imbalance handling, model training, hyperparameter tuning, ROC analysis, and dashboard visualisation in Power BI.

The project was developed in R and demonstrates end-to-end machine learning implementation for healthcare analytics.

---

## Objectives

- Predict stroke risk using supervised machine learning
- Compare multiple classification algorithms
- Handle class imbalance using resampling techniques
- Evaluate models using ROC-AUC and classification metrics
- Visualise insights using Power BI dashboards

---

## Dataset

Dataset: Stroke Prediction Dataset

Features include:

- Age
- Gender
- BMI
- Hypertension
- Heart disease
- Glucose level
- Smoking status
- Marital status
- Work type
- Residence type

Target Variable:

- `stroke`
  - 0 = No Stroke
  - 1 = Stroke

<img width="600" height="500" alt="image" src="https://github.com/user-attachments/assets/32e4a371-627f-4e41-8b39-3d6145735a0f" />

---

## Machine Learning Models Used

The following models were implemented and compared:

| Model | Purpose |
|---|---|
| Random Forest | Ensemble classification |
| Logistic Regression | Baseline statistical model |
| Decision Tree | Interpretable classification |
| Naive Bayes | Probabilistic learning |
| Support Vector Machine (SVM) | Margin-based classification |

---

## Resampling Techniques

Due to severe class imbalance in stroke cases, multiple balancing methods were applied:

- Upsampling
- Downsampling
- SMOTE
- ROSE

---

## Data Preprocessing

The preprocessing workflow included:

- Missing value handling using MICE imputation
- One-hot encoding of categorical variables
- Normalisation using Min-Max scaling
- Train-test splitting
- Feature engineering

---

## Model Evaluation Metrics

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Sensitivity
- Specificity
- ROC Curve
- Area Under Curve (AUC)

---

## ROC Curve Analysis

ROC curves were generated and compared across all machine learning models to evaluate classification performance and discriminative ability.

Example outputs include:

- ROC comparison plots
- Variable importance plots
- Confusion matrices
- Hyperparameter tuning plots

---

## Power BI Dashboard

An interactive Power BI dashboard was developed to visualise:

- Stroke prevalence
- Demographic distributions
- Feature importance
- Model performance metrics
- ROC-AUC comparisons
- Resampling effects

---

## Technologies Used

### Programming Language
- R

### Libraries
- caret
- tidyverse
- randomForest
- e1071
- mice
- pROC
- ROSE
- DMwR2
- plotly
- yardstick
- rpart

### Visualisation Tools
- ggplot2
- Plotly
- Power BI

---

## Project Structure

```text
Stroke-Prediction-ML/
│
├── data/
├── scripts/
├── outputs/
├── dashboard/
├── README.md
└── requirements.txt
```

---

## Key Findings

- Random Forest achieved the best predictive performance
- Class balancing significantly improved minority class detection
- BMI, age, and glucose level were strong predictors of stroke risk
- ROC-AUC analysis demonstrated improved classification after resampling

---

## Future Improvements

Potential future work includes:

- XGBoost implementation
- Deep learning models
- SHAP explainability
- Deployment using Shiny or Flask
- Real-time clinical risk scoring

---

## Author

Name: Bisona Honora

Field:
Health Data Science | Machine Learning | Epidemiology | Predictive Analytics

---

## License

This project is intended for academic, research, and portfolio purposes.
