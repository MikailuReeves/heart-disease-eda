[Dataset](https://www.kaggle.com/datasets/neurocipher/heartdisease/data) (now removed it seems)

# Heart Disease Prediction Project
## Overview

This project explores whether heart disease can be predicted using clinical and diagnostic measurements.

The goal was to:
- Identify which features are most strongly associated with heart disease.
- Build and evaluate predictive models.
- Interpret results in a practical and decision-oriented way.

## Methodology

Variables were classified by type (ratio, ordinal, binary). Univariate statistical tests were used to rank feature relevance.

## Modeling
Logistic Regression was the primary model where as Random Forest was the comparison model. Used:
- Stratified train/test split
- 5-fold cross-validation
- Evaluation using ROC-AUC, accuracy, and confusion matrices

## Most Influential Features
The strongest predictors were:
- ST depression
- Chest pain type
- Number of vessels (fluoroscopy)
- Thallium test results
- Maximum heart rate

Features such as fasting blood sugar, cholesterol, and resting blood pressure showed weak standalone association in this dataset.

## Results
Logistic Regression performance:
- Cross-validated ROC-AUC = 0.91
- Test ROC-AUC = 0.93
- Test accuracy = 0.87

Random Forest achieved similar performance but did not significantly outperform logistic regression.

## Limitations
The dataset is relatively small and very clean. And no external dataset was used to validate further.

Heart disease can be predicted using the available features. A simple logistic regression model performs well with this data.