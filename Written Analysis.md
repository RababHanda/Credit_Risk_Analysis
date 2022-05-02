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

<p align="center">
<img src="/Resources/naive.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 65%  |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 62%  <br>low risk: 68% | 

#### 2. SMOTE Oversampling

<p align="center">
<img src="/Resources/smote.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 64%  |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 63%  <br>low risk: 66% | 

#### 3. Undersampling

<p align="center">
<img src="/Resources/under.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 64%  |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 61%  <br>low risk: 45% | 

#### 4. Combination Under-Over Sampling

<p align="center">
<img src="/Resources/combo.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 53%  |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 70%  <br>low risk: 57% | 

#### 5. Balanced Random Forest Classifier

<p align="center">
<img src="/Resources/brfc.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 79%  |
| Precision | high risk: 9% <br>low risk: 100% | 
| Recall | high risk: 92%  <br>low risk: 94% | 

#### 6. Easy Ensemble Classifier

<p align="center">
<img src="/Resources/eec.png" width="70%" height="35%">
</p>

|  | **Scores** |
| --- | --- |
| Balanced Accuracy | 93%  |
| Precision | high risk: 9% <br>low risk: 100% | 
| Recall | high risk: 92%  <br>low risk: 94% | 

## Summary

| **Model** | **Conclusion** |
| --- | --- |
| Naive Random Oversampling | | 
| SMOTE Oversampling | | 
| Undersampling | | 
| Combination Under-Over Sampling | |
| Balanced Random Forest Classifier | |
| Easy Ensemble Classifier | |
