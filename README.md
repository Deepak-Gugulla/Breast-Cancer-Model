# Breast Cancer Study Analysis

This repository contains an analysis of breast cancer status based on a dataset from the German Breast Cancer Study Group (GBSG). The study examines factors associated with breast cancer recurrence or death and aims to predict patient outcomes using multiple logistic regression and other classification models.

## Dataset

The dataset used in this study is sourced from Kaggle:
[Breast Cancer Dataset - Royston and Altman](https://www.kaggle.com/datasets/utkarshx27/breast-cancer-dataset-used-royston-and-altman).

The dataset includes records from 686 patients who participated in a trial from 1984-1989, with the following key features:
- **meno**: Menopausal status (categorical)
- **size**: Tumor size (numeric, in mm)
- **grade**: Tumor grade
- **nodes**: Number of positive lymph nodes
- **pgr**: Progesterone receptor level (categorical)
- **er**: Estrogen receptor level (numeric)
- **hormon**: Hormonal therapy indicator (categorical)
- **rfstime**: Recurrence-free survival time (numeric, days)
- **status**: Outcome status (0 = alive without recurrence, 1 = recurrence or death)

## Analysis

The analysis focuses on predicting the outcome status (alive without recurrence vs. recurrence or death). Various methods and models were used:

### 1. Data Cleaning and Preparation
- Modified categorical variables for clarity.
- No missing or incomplete data points were found.

### 2. Graphical Analysis
- Explored relationships between survival time, tumor size, hormonal therapy, and breast cancer recurrence.

### 3. Primary Analysis: Multiple Logistic Regression
- Initially used eight predictors, followed by model selection based on Akaike Information Criteria (AIC) to identify significant predictors.
- Achieved a model accuracy of 68% and an AUC of 0.79.

### 4. Secondary Analysis: Other Models
- Tested additional models like Random Forest, C5.0, and Naive Bayes.
- Random Forest showed the highest accuracy.

### 5. Results
- Final model performance:
  - Accuracy: 68%
  - Sensitivity: 62%
  - Specificity: 74%
  - Area Under the Curve (AUC): 0.79

## Conclusions

The study identified menopause, tumor size, hormone therapy, and recurrence-free survival time as significant predictors of breast cancer recurrence or death. While the model demonstrated reasonable predictive power, further analysis and additional factors could improve accuracy.

## Future Work
- Explore more predictors and potential interactions.
- Try advanced machine learning techniques to enhance model performance.

## References
- Kaggle Dataset: [Breast Cancer Dataset](https://www.kaggle.com/datasets/utkarshx27/breast-cancer-dataset-used-royston-and-altman)

