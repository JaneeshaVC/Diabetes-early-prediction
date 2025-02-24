# Diabetes-early-prediction
Diabetes being a globally affecting non communicable disorder, is better if predicted early. 
Diabetes prediction using machine learning has become increasingly significant for early 
detection and prevention. This project evaluates various machine learning models, including 
Random Forest (RF), Decision Tree (DT), K-Nearest Neighbours (KNN), and Logistic 
Regression (LR) and Naïve Bayers (NB) to determine their predictive accuracy for diabetes 
diagnosis. Model performance was assessed using accuracy, precision, recall, F1-score, and 
ROC-AUC. To enhance prediction accuracy, feature selection techniques such as Recursive 
Feature Elimination (RFE), VIF, Chi square test were applied. 

# Introduction
Diabetes being the most common and the deadliest non communicable disease in the world, 
globally affects around 537 million people at present, forecasting to reach 642 million, in 2040. 
Insulin, being a major factorial in the human body, is responsible to maintain the blood glucose 
levels, normal. However, due to defective insulin secretions, impaired biological synthesis or 
resistance, the blood glucose levels could change drastically causing high levels of glucose in 
blood, hence leading to conditions called Diabetes.Early diagnosis and intervention are essential in preventing the progression of diabetes, mitigating its impact, and improving patient quality of life. Addressing the lack of awareness and the delayed diagnosis is a significant challenge in modern healthcare. Current diagnostic methods, while effective, are often time consuming, costly, and require a clinical setting to perform tests such as blood glucose level 
assessments. Therefore, there is a growing need for innovative solutions that can facilitate the early identification of individuals at risk of developing diabetes.

# Aim of the project
The aim of this project is to develop a machine learning model to predict the likelihood of diabetes in individuals using medical data

# Methodology
1. Dataset Collection and Preparation
Dataset was retrieved from Kaggle and provided for open access. 
Irrelevant columns were removed, including AnyHealthcare, 
NoDocbcCost, GenHlth, PhysHlth, Education, and Income. After cleaning, the dataset was 
reviewed for its shape (rows and columns), with the first five rows of the dataset.

2. Statistical Summary and Null value check 
No null values found, further examine on the presence of 
any duplicates, were considered. 121509 duplicate records were identified and were removed 
to ensure data consistency and accuracy.

3. Outlier Detection
Boxplots were used to identify potential outliers in the dataset. 
The outliers were detected only in BMI and in MentHlth, where the outliers in the BMI column 
were removed based on the Interquartile Range (IQR) method. The outliers of the MentHlth were ignored.

4. Data Splitting
The data was split into 80/20 split.

5. Class balancing and feature scaling 
To address the class imbalance in the target variable (Outcome), SMOTE (Synthetic Minority 
Over-sampling Technique), leaving the testing data unaffected. 

