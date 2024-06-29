# Maternal-Health-Python-Project

# Project Report: Analysis of Maternal Pregnancy Risk Factors

## Introduction

This report presents an exploratory analysis of maternal pregnancy risk factors based on a dataset from a medical study. The dataset includes various physiological measurements and demographic information related to pregnant individuals.

## Data Exploration and Cleaning

The project began by importing necessary libraries and loading the dataset from a CSV file. Initial exploration involved printing data summaries, identifying null values, and converting relevant columns to numeric format. Null values were replaced with column means to ensure data integrity.

## Outlier Handling

Outliers were identified visually through boxplots, specifically noting significant outliers in the 'Age' and 'DiastolicBP' columns. An outlier in 'DiastolicBP' (1000) was corrected based on clinical judgment, while outliers in 'Age' (extremes like giving birth at 10 or 70) were retained considering medical feasibility.

## Feature Engineering

A new feature, 'Adjusted_BS', was derived by subtracting 3 from the 'BS' (Blood Sugar) column, which was subsequently dropped. The 'RiskLevel' column was standardized by capitalizing its values for consistency.

## Exploratory Data Analysis

A correlation matrix was generated and visualised using a heatmap to explore relationships between variables. Key findings included a medium positive correlation between 'Age' and 'Adjusted_BS', and between systolic and diastolic blood pressure ('SystolicBP' and 'DiastolicBP').

## Insights from Visualizations

- **Age vs. Risk Level**: Boxplots showed that high-risk pregnancies tend to occur at older ages (median around 35), while low-risk pregnancies are associated with younger ages (early 20s).
  
- **Risk Level Distribution**: A pie chart illustrated that the majority of pregnancies were categorized as low risk, followed by high-risk and mid-risk pregnancies.

- **Scatter Plots**: Scatter plots indicated a positive correlation between 'Adjusted_BS' (Blood Sugar) and maternal age, as well as between 'SystolicBP' and 'DiastolicBP', aligning with medical expectations.

## Conclusion

This project provided valuable insights into maternal pregnancy risk factors. The analysis highlighted the role of age in influencing blood sugar levels and blood pressure during pregnancy. Understanding these factors can contribute to better healthcare management and risk assessment for pregnant individuals.

## Future Directions

Future analyses could delve deeper into specific risk factors affecting different age groups or explore additional variables that may impact pregnancy outcomes. Moreover, machine learning models could be applied to predict pregnancy risk levels based on the identified factors.

## References

- Python libraries: Pandas, NumPy, Matplotlib, Seaborn

