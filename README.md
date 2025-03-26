# Comprehensive Feature Predictive Power Analysis and Selection

## Project Summary

This notebook provides a comprehensive evaluation of feature predictive power (in this example for fraud detection models) by integrating exploratory data analysis, advanced statistical metrics, and machine learning techniques. The analysis is structured into seven sections, each contributing key insights into feature performance:

## Sections

### 1. EDA and Feature Overview
- Summarizes each feature's characteristics, including type, missing values, cardinality, and detailed descriptive statistics for numeric features (with outlier detection).
- Categorical features are preserved in their raw form for summary purposes and then transformed for visual and predictive analysis.

### 2. Visual Distribution and Relationship Plots
- Uses histograms or bar plots to display feature distributions.
- Boxplots to show the relationship between features and the fraud target.
- Binned fraud rate charts to reveal how fraud rates vary across feature intervals.

### 3. Advanced Performance Visualizations
- Provides PSI plots to assess distribution stability between datasets.
- Lift charts to evaluate segmentation power.
- PR-AUC curves along with key classification metrics (Precision, Recall, F1 Score) to measure predictive performance.

### 4. WOE and IV Analysis
- Breaks down features into bins and calculates Weight of Evidence (WOE) and Information Value (IV) to quantify how well each feature distinguishes between fraudulent and non-fraudulent cases.
- Scaled IV values are computed to facilitate direct comparisons across features.

### 5. Extra Categorical Metrics
- Augments the analysis with additional metrics such as:
  - Chi-Square P-Value
  - Cramér’s V
  - Mutual Information
  - Gini Index
  - ReliefF Score
  - Information Gain
- These metrics further support the evaluation of categorical feature performance.

### 6. Feature Correlations Analysis
- Examines the correlation matrix to identify and flag highly correlated features (with near-perfect correlations) as candidates for removal.
- Helps to mitigate multicollinearity and streamline the feature set.

### 7. Combined Feature Importance Analysis using LightGBM and SHAP
- Executes multiple runs of a LightGBM classifier on the training data and employs SHAP values to rank features based on their predictive contribution.
- The aggregated, scaled SHAP values provide actionable insights into which features are most influential for detecting fraud.

## Conclusion
This notebook systematically combines statistical summaries, visualization techniques, and model-based metrics to determine the most effective features for fraud detection in card transactions. By evaluating features comprehensively—from data quality and distribution stability to their direct influence on predictive performance—the analysis ensures the final selected features form a robust, accurate, and reliable foundation for high-performing fraud detection models and rule development.

## Notes
- *Example outputs are provided in each section to illustrate the expected results.*
- *This specific notebook is based on fraud detection for card transaction data.*
