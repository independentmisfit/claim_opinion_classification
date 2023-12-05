# claim_opinion_classification
# TikTok Claims Classification Project: README
## Overview
The TikTok Claims Classification Project aims to develop a machine learning model for accurately categorizing claims within user submissions. The project encompasses various phases such as data inspection, exploratory analysis, statistical tests, regression analysis, and machine learning model development.
## Business Problem
The primary objective is to assist the TikTok data team in building a robust model capable of effectively categorizing user claims. These insights will aid in prioritizing videos for review, ensuring compliance with the platform's terms of service.
## Milestones Summary:
### Milestone 1: Data Inspection and Understanding
The preliminary investigation focused on understanding relationships between variables in the dataset. Key insights included:

A near balance between counts of claims and opinions in the dataset.
Identification of crucial variables: video duration and view count, critical for future prediction models.
### Milestone 2: Exploratory Data Analysis (EDA)
During the EDA phase, visualization of data provided deeper insights:

Addressing null values, imbalances in opinions, and skewed data distributions.
Observations included missing values and skewed data distributions in view and like counts, impacting model construction.
### Milestone 3: Statistical Test on Verified Status and View Counts
An independent sample  t-test was conducted to analyze the relationship between verified status and video view counts. The findings suggested:

A significant difference in view counts between verified and unverified accounts, indicating potential behavioral differences.
Recommendations for further investigation into behavioral distinctions among account types.
Interpretation of Statistical Test:
The independent sample t-test involving verified status and video view counts revealed a substantial difference between the mean view counts of verified and unverified accounts. The observed difference in the sample data indicated a potential divergence in engagement levels between these account types. Further exploration is recommended to understand the behavioral disparities influencing view counts.

### Milestone 4: Regression Analysis on Verified Status
A logistic regression model was built to predict verified status, revealing:

Lengthier videos tend to be associated with higher odds of users being verified.
Other video features show smaller associations with verified status, influencing the subsequent claim classification model.
Interpretation of Logistic Regression Model:
The logistic regression analysis identified video duration as a significant predictor of verified status, indicating higher odds of verification for longer videos. While other video features exhibited smaller associations, the emphasis on video length suggests its importance in influencing user verification status.

### Milestone 5: Machine Learning Model Development
Developed tree-based classification models (Random Forest and XGBoost) to predict claim status. Highlights include:

Selection of the Random Forest model as the champion model based on its superior recall score of 0.99.
Achieved near-perfect performance on the test dataset, attributing predictive signals primarily to engagement metrics.

## Factors Determining Claim or Opinion Status:
Several factors significantly influence the categorization of posts as either claims or opinions:

Video Engagement Metrics: Metrics such as video view count, like count, share count, and download count play crucial roles in distinguishing claims from opinions. Higher engagement levels are more indicative of claim status.
Video Duration: Longer videos tend to be associated with higher odds of being classified as claims.
User Verification Status: Verified accounts may exhibit different posting behaviors influencing the type of content they share.
Null Values: Over 200 null values in various columns impact the insights derived and need consideration in model construction and analysis.
![feature importance tiktok](https://github.com/independentmisfit/claim_opinion_classification/assets/112862611/3531fa95-7dda-48e6-8cd5-537c21d7c2a1)

### Conclusion and Recommendations
The TikTok Claims Classification Project covers a comprehensive analysis of user-submitted content, leveraging statistical and machine learning techniques. The chosen champion model, the Random Forest, stands out based on its exceptional recall score, indicating superior performance in identifying claims. Various engagement metrics and user-related features significantly contribute to distinguishing between claims and opinions. Recommendations include continuous monitoring of engagement metrics and model refinement for improved accuracy and performance.

This README provides an overview of the project's significant milestones, statistical test interpretations, logistic regression insights, and factors influencing claim classification. Further details and code implementations can be found in the project documentation and associated notebooks.
