# Bank-Churn-Predictive-Analytics
Predicting customer defection using Random Forest and Decision Tree classifiers.

Bank Customer Churn: Predictive Modeling & Analysis 

Project Overview 

This project addresses the challenge of predicting client churn to help banks assess risk and improve customer retention. Using a dataset of 10,127 clients, I developed a machine learning pipeline to identify key factors influencing bank turnover.

Data Synthesis & Preprocessing

To ensure model integrity and computational efficiency, I performed the following steps:

Null Value Handling: Used the .isnull().sum() and .dropna() methods to verify and ensure zero missing values within the dataset.
Feature Pruning: Identified and removed redundant columns, including the unique CLIENTNUM and two Naïve Bayes classifier columns provided by the original dataset author.

![Data Cleaning and Synthesis Step](data-cleaning-synthesis.png)

Data Inspection & Distribution

Before engineering features, I inspected the underlying structure and class balance of the dataset.

Statistical Summary: Utilized .describe() and .info() to identify variable types and check for anomalies in the numeric features.

Class Balance Check: Performed .value_counts() on categorical columns to understand the distribution of the target label (Attrition_Flag) and other key demographics like Income_Category and Education_Level.

![Data Inspection and Distribution Step](data-inspection.png)

Feature Engineering & Categorical Encoding

To prepare the data for the Random Forest and Decision Tree classifiers, I transformed text-based categories into numerical formats.

Ordinal Encoding: Manually mapped ranked variables such as Education_Level, Income_Category, and Card_Category to a numeric scale (e.g., Graduate = 4, Doctorate = 6).

One-Hot Encoding: Used pd.get_dummies for nominal variables like Gender and Marital_Status to create binary identifiers, ensuring the model treats them as distinct categories without an inherent rank.

Data Integration: Concatenated the newly encoded features back into the primary dataframe and removed the original text columns to finalize the feature set.

![Feature Engineering & Categorical Encoding Step](feature-encoding.png)
