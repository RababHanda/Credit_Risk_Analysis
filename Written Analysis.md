# Credit_Risk_Analysis

## Overview of Project
This project analyzes the reveiws on furniture products provided by Amazon Vine

### Purpose

**Analytical:**  

**Technical:** packages - NumPy, numpy-base, numpydoc, SciPy, Scikit-learn


## Results

Results for each specific score can be seen from the resampling code [^1]

[^1]: `https://github.com/RababHanda/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb`


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

| **Model** | **Conclusion** |
| --- | --- |
| Naive Random Oversampling | The precision for high-risk loan applications is extremely low (at 1%)<br> The accuracy is at par for both high and low risk loans, averaging to 66% | 
| SMOTE Oversampling | The precision for high-risk loan applications is extremely low <br> The accuracy is average for both high and low risk loans (in the 60s range) | 
| Undersampling | The precision for high-risk loan applications is extremely low <br> The accuracy is low for high risk loans (45%) and average for low risk loans (61%) | 
| Combination Under-Over Sampling | The precision for high-risk loan applications is extremely low <br> The accuracy good for high risk loans (70%) and average for low risk loans (57%) |
| Balanced Random Forest Classifier | The precision for high-risk loan applications is low (9%) <br> The accuracy very high for both, high & low risk, loan applications, averaging to 94% |
| Easy Ensemble Classifier | The precision for high-risk loan applications is low (9%) <br> The accuracy very high for both, high & low risk, loan applications, averaging to 94% |
