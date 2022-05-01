# Credit_Risk_Analysis

## Overview of Project
This project analyzes the reveiws on furniture products provided by Amazon Vine

### Purpose

**Analytical:**  

**Technical:** packages - NumPy, numpy-base, numpydoc, SciPy, Scikit-learn


## Results

Results for each specific score can be seen from the resampling code [^1]

[^1]: `https://github.com/RababHanda/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb`

<p align="center">
<img src="/Resources/naive.png" width="60%" height="30%">
</p>

#### 1. Naive Random Oversampling
|  | Balanced Accuracy Scores |
| Balanced Accuracy Score | 65%  |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 62%  <br>low risk: 68% | 

#### 2. SMOTE Oversampling
|  | Balanced Accuracy Scores |
| Balanced Accuracy Score | 65%  |
| Precision | high risk: 1% <br>low risk: 100% | 
| Recall | high risk: 62%  <br>low risk: 68% | 

#### 3. Undersampling

#### 4. Combination Under-Over Sampling

#### 5. Balanced Random Forest Classifier

#### 6. Easy Ensemble Classifier


<p align="center"><span class="emphasized"> Table 1. Summary of "Helpful" Votes </span></p>
<p align="center">
<img src="/Resources/helpful_summary_df.png" width="60%" height="30%">
</p>

<p align="center"><span class="emphasized"> Table 2. Summary of All Votes </span></p>
<p align="center">
<img src="/Resources/all_summary_df.png" width="60%" height="30%">
</p>


#### 1. How many Vine reviews and non-Vine reviews were there?
In total there are 792,113 reviews, of which 2,775 are Vine and 789,338 are non-Vine. 
However, among the "voted" reveiws, there here are 130 Vine reviews and 16,820 non-Vine reviews. (*similar breakdown*)

#### 2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
There were 1,356 5-star Vine reviews and 446,360 5-star non-Vine reviews. 
For reviews voted "helpful", there are 70 Vine and 7,957 non-Vine 5-star reveiws. (*similar breakdown*)

#### 3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
49% of the total Vine reviews are rated 5 stars, whereas 56.5% of all non-Vine reviews are rated 5 stars. 
For reviews voted "helpful", of 54% Vine and 47% of non-Vine reviews are rated 5 stars. (*similar breakdown*)

## Summary

Of the total 792,113 reviews 56.5% are rated at 5 stars (comprising 447,716 reviews). 
<p align="center">
<img src="/Resources/5star_summary_df.png" width="40%" height="25%">
</p>

Of these 447,716 only 1,356 come from paying members and 446,360 come from non-paying members. But when comparing the percentages of 5 stars from each type of reviews (paid vs unpaid) the results are approximately equal (49% vs 56.5%), therefore it can be confidently concluded members review products just like non memebers. A paid review isn't skewed compared to an unpaid one. Refering to tables 1 & 2 in the previous section, the "helpful" reviews also follow the same breakdown pattern as all review, so this further assures that reviews aren't biased as they are spread out the same way. 

However, when comparing the breakdown of reviews coming from different types of members it can be noted that people tend to give 5 star ratings more than any other rating. It is possible that the product really is good and that is reflected in the ratings, however further investigation can be done to see if giving 5-star reviews helps customers in any way.
