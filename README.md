# Fifa-s4ds

## **FIFA Player Analysis & Overall Rating Prediction**

This project focuses on Exploratory Data Analysis (EDA) and predictive modeling using FIFA player datasets (2017–2022). 
The goal is to understand player attributes, identify patterns, and predict the Overall Rating of a player.

## **Key Steps in the Workflow**

### **Data Cleaning & Preprocessing**

- Removed noise from player names (special characters, numbers, whitespace).
- Handled missing values, NaNs, and inconsistent encodings.
- Converted categorical monetary values (€, K, M) into numeric player values in Euros.
- Explored outliers and applied RobustScaler for handling skewed distributions.

### **Exploratory Data Analysis (EDA)**

- Plotted distributions of 30+ features to study skewness, modality, and value ranges.
- Used boxplots and violin plots to highlight outliers and distributions.
- Visualized hexbin plots for relationships between key technical attributes (e.g., Finishing vs Composure).
- Built correlation heatmaps to study linear dependencies across player features.
- Analyzed club strengths across seasons (2017–2022) by comparing mean overall ratings.
- Studied top 5 players’ progression in terms of Overall & Market Value.

### **Feature Engineering & Selection**

- Identified irrelevant features for predicting Overall (e.g., GK attributes negatively correlated with Outfield features).
- Performed outlier detection using IQR and evaluated transformations.

### **Modeling**

- Built RandomForestRegressor to predict a player’s Overall Rating from their attributes.
- Achieved R² > 0.96 and very low RMSE, showing strong predictive performance.
- Performed Cross-Validation to check model stability (proved no overfitting).
- Interpreted results using feature importance ranking to understand which skills matter most.

## **Outcomes**

- A complete EDA-to-Model pipeline on FIFA player data.
- Insights into player development, club strength trends, and skill correlations.
- A reliable predictive model for player Overall Rating, interpretable through feature importances.
