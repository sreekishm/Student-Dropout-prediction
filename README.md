# Student-Dropout-prediction
## Overview
Student dropout is a major challenge for educational institutions. Early identification of students at risk of dropping out enables institutions to intervene and improve retention rates.

This project develops a machine learning pipeline to predict student dropout and academic outcomes using demographic, academic, and socioeconomic factors. The approach combines clustering, class imbalance handling, and explainable machine learning models to generate actionable insights.
# Project Objectives
- Identify students at risk of dropping out.
- Segment students into meaningful groups using clustering.
- Train specialized machine learning models for each segment.
- Improve prediction accuracy compared to a single global model.
- Provide explainable insights into factors influencing dropout.
# Dataset
## Demographic Features
- Marital Status
- Nationality
- Gender
- Age at enrollment
## Academic Background
- Previous Qualification
- Previous Qualification Grade
- Admission Grade
- Course Enrolled
- Attendance Type
## Family & Socioeconomic Factors
- Mother's Qualification
- Father's Qualification
- Mother's Occupation
- Father's Occupation
## Academic Performance Indicators
- Curricular units (credited, enrolled, approved)
- Evaluation grades
- Semester performance metrics
## Target Variable
The model predicts student academic outcomes, including:
- Dropout
- Enrolled
- Graduate
# Project Workflow
## Data Preprocessing
- Loading dataset
- Checking data structure and types
- Handling categorical variables
- Verifying missing values
- Converting numeric encoded categories to categorical features
## Exploratory Data Analysis (EDA)
- Distribution of student outcomes
- Relationships between academic performance and dropout
- Impact of demographic and socioeconomic variables
## Feature Engineering
- Encoding categorical variables
- Scaling numerical features using StandardScaler
- Preparing features for clustering and modeling
## Handling Class Imbalance
- SMOTE (Synthetic Minority Oversampling Technique)
## Feature Selection
- Feature selection was performed to identify the most relevant predictors influencing student outcomes.
## Student Segmentation using Clustering
- Instead of using a single model for all students, the dataset was segmented using DBSCAN clustering.
## Cluster-Specific Machine Learning Models
- Separate Random Forest models were trained for each cluster.
## Model Explainability
- To understand model decisions, SHAP (SHapley Additive Explanations) was used.
# Technologies Used
## Programming
- Python
## Libraries
- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn
- imbalanced-learn
- SHAP
## Machine Learning Techniques
- SMOTE (class imbalance handling)
- DBSCAN (clustering)
- Random Forest (classification)
- SHAP (model explainability)
