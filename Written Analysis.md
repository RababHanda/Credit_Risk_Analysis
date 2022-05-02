# Credit_Risk_Analysis

## Overview of Project
In this project I analyze 6 different models for sampling data for credit card applications, to analyze whether or not the applicants qualify.

### Purpose

**Analytical:** I deply supervised machine learning models to determine the eligibility of applicants for credit card loans. I analyze the confusion matrix to determine false negatives/positives and true negatives/positives to understand the precision and accuracy of each model

**Technical:** packages - numpy, numpy-base, numpydoc <br> Libraries: NumPy, SciPy, Scikit-learn, Pandas


## Results


#### 1. Naive Random Oversampling

<p align="left">
<img src="/Resources/naive.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 65% [^1] |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 62%  <br>low risk: 68% | 

#### 2. SMOTE Oversampling

<p align="left">
<img src="/Resources/smote.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 64% [^1] |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 63%  <br>low risk: 66% | 

#### 3. Undersampling

<p align="left">
<img src="/Resources/under.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 64% [^1] |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 61%  <br>low risk: 45% | 

#### 4. Combination Under-Over Sampling

<p align="left">
<img src="/Resources/combo.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 53% [^1] |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 70%  <br>low risk: 57% | 

[^1]: `https://github.com/RababHanda/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb`

#### 5. Balanced Random Forest Classifier

<p align="left">
<img src="/Resources/brfc.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 79% [^2] |
| Precision | high risk: 9% <br>low risk: 100% | 
| Recall | high risk: 92%  <br>low risk: 94% | 

#### 6. Easy Ensemble Classifier

<p align="left">
<img src="/Resources/eec.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 93% [^2] |
| Precision | high risk: 9% <br>low risk: 100% | 
| Recall | high risk: 92%  <br>low risk: 94% | 

[^2]: `https://github.com/RababHanda/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb`

## Summary

The scores for high risk loans will be used to compare the different models because that is the constraint that will majorly affect the company giving out loans. Cost of low risk applicants being wrongly determined eligible won't pose much of a risk to the company.

| **Model** | **Conclusion** |
| --- | --- |
| Naive Random Oversampling | The precision for high-risk loan applications is extremely low (at 1%)<br> The accuracy is at par for both high and low risk loans, averaging to 66% | 
| SMOTE Oversampling | The precision for high-risk loan applications is extremely low <br> The accuracy is average for both high and low risk loans (in the 60s range) | 
| Undersampling | The precision for high-risk loan applications is extremely low <br> The accuracy is low for high risk loans (45%) and average for low risk loans (61%) | 
| Combination Under-Over Sampling | The precision for high-risk loan applications is extremely low <br> The accuracy good for high risk loans (70%) and average for low risk loans (57%) |
| Balanced Random Forest Classifier | The precision for high-risk loan applications is low (9%) <br> The accuracy very high for both, high & low risk, loan applications, averaging to 94% |
| Easy Ensemble Classifier | The precision for high-risk loan applications is low (9%) <br> The accuracy very high for both, high & low risk, loan applications, averaging to 94% |

1. As seen in the section above, Easy Ensemble Classifier has the highest accuracy score - at 93%, among the 6 different sampling models. The acuracy score stand-alone is also very high in terms of acceptability (over 80%).
2. Easy Ensemble Classifier and Balanced Randon Forest Classifier both have the higher precision rate for high-risk applications (even though it is low in terms of stand alone percentages, it is comparably higher among the sox models)
3. Easy Ensemble Classifier and Balanced Randon Forest Classifier both have recall scores in low 90s, however high risk application have higher recall score in Easy Ensemble Classifier (94%). 

**Final Conclusion**: Looking at all 3 critereon, ***Easy Ensemble Classifier*** model provides the highest level level of accuracy overall and for high risk loans. It also provides higher precision rate among all models for high risk applications