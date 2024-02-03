# Credit Card Fraud Detection and Sampling Techniques Evaluation

## Introduction

This repository contains Python code for analyzing credit card fraud data and evaluating various sampling techniques for imbalanced datasets. The script utilizes the Pandas library for data manipulation, Seaborn for data visualization, scikit-learn for machine learning models, and imbalanced-learn (imblearn) for sampling techniques.

## Dataset

The credit card fraud dataset used in this analysis is stored in a CSV file named Creditcard_data.csv. This dataset contains features related to credit card transactions, including transaction amount, time, and other anonymized features. The target variable Class indicates whether a transaction is fraudulent or not.

## Sampling Techniques

The script evaluates the performance of several sampling techniques to handle class imbalance, including:

- RandomOverSampler
- SMOTE (Synthetic Minority Over-sampling Technique)
- EditedNearestNeighbours
- RandomUnderSampler
- ClusterCentroids
- SMOTEENN (SMOTE + Edited Nearest Neighbors)

## Code Structure

- Data Loading: The script loads the credit card fraud dataset using Pandas.
- Data Visualization: It visualizes the class distribution using a bar plot before and after applying oversampling techniques.
- Sampling Techniques and Model Training: It applies the defined sampling techniques to create balanced datasets and trains machine learning models on each sample.
- Model Evaluation: The accuracy of each model trained on different sampling techniques is recorded and stored in a Pandas DataFrame.
- Results Saving: The results of model evaluation, including model names and their corresponding accuracies, are saved in a CSV file named accuracy_results.csv.

## ML models used

- DecisionTreeClassifier
- RandomForestClassifier
- SVC
- DecisionTreeClassifier
- RandomForestClassifier

## How to Use

1. Ensure you have Python installed on your system.
2. Install the required libraries by running pip install pandas seaborn scikit-learn imbalanced-learn in your terminal.
3. Run the Python script in your preferred environment.
4. Review the generated accuracy results CSV file for model performance under different sampling techniques.

## Note

This script assumes that the credit card fraud dataset is located at /Users/rishavjain/Desktop/sampling/Creditcard_data.csv. Please adjust the file path accordingly.
Adjust the sample size detection formula based on your requirements.
You can modify the list of sampling techniques and machine learning models according to your preference.