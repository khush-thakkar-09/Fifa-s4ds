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

### Interactive Plots Pictures:- (since you cannot see them in the notebook)

<img width="655" height="316" alt="Screenshot 2025-09-23 at 1 48 38 AM" src="https://github.com/user-attachments/assets/93f8dc49-a3ad-485f-b708-1a8af82caea4" />

<img width="664" height="317" alt="Screenshot 2025-09-23 at 1 49 02 AM" src="https://github.com/user-attachments/assets/e2a66052-78dc-4fbf-b097-4ede0e47624c" />

<img width="673" height="303" alt="Screenshot 2025-09-23 at 1 49 20 AM" src="https://github.com/user-attachments/assets/89069f8d-b5cd-4f84-bc69-e581a114b197" />
