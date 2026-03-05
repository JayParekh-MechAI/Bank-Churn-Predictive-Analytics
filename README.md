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
