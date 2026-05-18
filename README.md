# Stroke Prediction Using Machine Learning

## Project Overview

This project applies machine learning techniques to predict stroke occurrence using demographic and clinical data. The workflow includes data preprocessing, missing-value imputation, class-imbalance handling, model training, hyperparameter tuning, and ROC analysis. 

The project was developed in R and demonstrates end-to-end machine learning implementation for healthcare analytics.

---

## Objectives

- Handle class imbalance using resampling techniques
- Predict stroke risk using supervised machine learning
- Compare multiple classification algorithms
- Evaluate models using ROC-AUC and classification metrics
- Significance of results to epidemiology and health science

---

## Dataset
The dataset contains patient demographic and clinical features used to predict stroke occurrence.
Source: Kaggle Stroke Prediction Dataset

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
  
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/32e4a371-627f-4e41-8b39-3d6145735a0f" />

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/5a87418c-cf31-4699-91fb-e4b65f01747f" />

Target Variable:

- `stroke`
  - 0 = No Stroke
  - 1 = Stroke

---
## Data Preprocessing

The preprocessing workflow included:

- Missing value handling using MICE imputation
- One-hot encoding of categorical variables
- Normalisation using Min-Max scaling
- Train-test splitting
- Feature engineering
  
---

## Resampling Techniques

Due to severe class imbalance in stroke cases (Shiny was used to generate the image in R): 
<img width="450" height="400" alt="image" src="https://github.com/user-attachments/assets/914a8555-83a0-43d2-88ca-7e7e22e07cba" />


Multiple balancing methods were applied to the training data after the split
- Upsampling (Random Oversampling (ROS))
- Downsampling (Random Under-sampling (RUS))
- SMOTE (Synthetic Minority Oversampling Technique)
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/bb73a24c-273f-4627-910f-0bdf5ce95801" />

---
## Machine Learning Models Used

The following models were implemented and compared:

| Model | Purpose |
|---|---|
| Random Forest | Ensemble classification |
| Logistic Regression | Baseline statistical model |
| Naive Bayes | Probabilistic learning |
| Support Vector Machine (SVM) | Margin-based classification |

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

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/e6fd97ba-7529-46a4-ad31-567ad4c2902a" />
<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/9f533dbd-4e59-48e7-9eea-4527d4ac551e" />
<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/95c51f5f-53bd-4416-a610-f367efb88666" />

---

## Technologies Used

### Programming Language
- R

### Visualisation Tools
- ggplot2
- Plotly
- Shiny

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
## Key Findings

- Random Forest achieved the best predictive performance
- Class balancing significantly improved minority class detection
- BMI, age, and glucose level were strong predictors of stroke risk
- ROC-AUC analysis demonstrated improved classification after resampling


## Significance of work to health Science and to Epidemiology

Stroke remains a leading cause of mortality and long-term disability worldwide. Early detection models can support clinical decision-making, enabling preventive interventions for high-risk patients. The integration of machine learning methods into healthcare analytics allows for improved risk stratification using routinely collected clinical data. Such models can assist healthcare systems in identifying at-risk populations, optimising resource allocation, and improving preventive care strategies. Furthermore, the methodological framework used in this study- combining resampling techniques, ensemble and nonlinear classifiers- can be extended to other disease prediction problems such as cardiovascular disease, diabetes, and infectious disease forecasting.

---
## Author

Name: Bisona Honora

Field:
Health Data Science | Machine Learning | Epidemiology | Predictive Analytics

---

## License

This project is intended for academic, research, and portfolio purposes.
