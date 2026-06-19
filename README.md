##ShopSmart: E-Commerce Purchase Prediction
#Overview

ShopSmart is a machine learning project focused on predicting whether a visitor to an e-commerce website will complete a purchase based on their browsing behavior during a session.

The goal is to help businesses identify high-intent visitors, optimize marketing strategies, and improve conversion rates by leveraging data-driven insights.

#Problem Statement

E-commerce platforms receive thousands of visitors daily, but only a fraction of them complete a purchase. Understanding customer behavior and predicting purchase intent can help businesses:

-Improve targeted marketing campaigns
-Increase conversion rates
-Reduce customer acquisition costs
-Enhance user experience

This project builds a predictive model that determines whether a visitor is likely to make a purchase based on session-level browsing data.

#Dataset

The dataset contains information from 12,330 unique user sessions collected over a one-year period.

Each session includes a combination of:

Numerical Features
-Administrative Duration
-Informational Duration
-Product Related Duration
-Bounce Rates
-Exit Rates
-Page Values
-Special Day Score

Categorical Features
-Month
-Visitor Type
-Weekend
-Operating System
-Browser
-Region
-Traffic Type

Target Variable
Revenue
True → Purchase Completed
False → No Purchase

#Project Workflow
-Data Understanding
-Exploratory Data Analysis (EDA)
-Data Preprocessing
-Feature Engineering
-Train-Test Split using Stratification
-Model Building
-Hyperparameter Tuning
-Model Evaluation
-Model Selection

#Data Preprocessing

The following preprocessing techniques were applied:

- Missing value inspection
- Numerical feature scaling using StandardScaler
- Categorical feature encoding using OneHotEncoder
- ColumnTransformer for combined preprocessing
- Pipeline implementation for reproducible workflows

#Machine Learning Models
Logistic Regression

Used as a baseline classification model.

Advantages:

-Fast and interpretable
-Strong baseline for binary classification

Decision Tree Classifier

Used to capture non-linear relationships and complex decision boundaries in customer behavior data.

Advantages:

-Easy to interpret
-Handles feature interactions effectively
-Performs well on structured tabular datasets

#Hyperparameter Tuning

Decision Tree hyperparameters were optimized using GridSearchCV with 5-Fold Cross Validation.

Parameters tuned:

-max_depth
-min_samples_leaf

Evaluation Metric:

-F1 Score

#Model Evaluation

Models were evaluated using:

-Accuracy
-Precision
-Recall
-F1 Score
-Confusion Matrix
-Classification Report

Since purchase prediction is an imbalanced classification problem, F1 Score was used as the primary evaluation metric.

#Results

Model Comparison:

Model	Purpose
Logistic Regression	- Baseline Model
Decision Tree	Final - Selected Model

Best Model

Decision Tree Classifier

The Decision Tree outperformed Logistic Regression in terms of F1 Score and was selected as the final model.

Hyperparameter tuning further improved the model's performance through cross-validation.

#Technologies Used
-Python
-Pandas
-NumPy
-Matplotlib
-Seaborn
-Scikit-Learn
-Jupyter Notebook

#Key Learnings

Through this project, I learned:

-Handling mixed numerical and categorical features
-Building preprocessing pipelines
-Feature scaling and encoding
-Stratified train-test splitting
-Logistic Regression
-Decision Trees
-Hyperparameter tuning using GridSearchCV
-Cross-validation
-Evaluating imbalanced classification problems using F1 Score

#Future Improvements

-Random Forest Classifier
-XGBoost
-Feature importance analysis
-Advanced feature engineering
-Model deployment using Streamlit
-Real-time purchase intent prediction dashboard

#Author

Shaina Noushad

B.Tech CSE (AI & ML)
