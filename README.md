## Project Overview
This project focuses on evaluating employees for potential layoffs due to a financial crisis faced by a company with over 4,000 employees. The goal is to reduce costs while minimizing the impact on company operations.

## Objectives
1. Analyze the characteristics and performance of employees.
2. Develop a model to identify employees for potential layoffs.
3. Provide recommendations to minimize the impact on company operations.

## Context
The dataset includes information on all employees of the company in 2015, with fixed working hours of 8 hours/day. The data consists of 6 tables and 24 columns, which were consolidated into one table containing the important attributes.

### Key Attributes
- **Skill Score**: Assessed based on education, monthly income, and percent salary hike.
- **Will Score**: Assessed based on working hours, career path, and satisfaction score.
- **Employee Segments**: Based on Skill and Will scores, employees are segmented into four categories:
  - **A**: High Skill / High Will
  - **B**: High Skill / Low Will
  - **C**: Low Skill / High Will
  - **D**: Low Skill / Low Will

## Methodology
1. **Data Collection and Preprocessing:**
   - Clean the data and handle duplicates and null values.
   - Convert categorical data into numerical format suitable for analysis.

2. **Exploratory Data Analysis (EDA):**
   - Analyze the overall performance and characteristics of employees.
   - Segment employees based on Skill and Will scores.

3. **Employee Segmentation:**
   - Segment employees into four groups based on their Skill and Will scores.
   - Identify employees in the Low Skill / Low Will group (Group C) for potential layoffs.

4. **Model Building and Evaluation:**
   - Develop machine learning models to predict employee performance and identify potential layoffs.
   - Evaluate models based on precision, recall, F1-score, and other relevant metrics.

## Key Findings
1. **High-Risk Employees:**
   - Employees in Group C (Low Skill / Low Will) are prioritized for layoffs.
   - Employees with high education but low contribution to the company are also considered for layoffs.

2. **Model Performance:**
   - The XGBoost model showed the highest performance in predicting employee performance and potential layoffs.
   - Logistic Regression and Decision Tree models also performed well but require further optimization.

## Recommendations
1. **For Group C Employees:**
   - Prioritize layoffs for employees in Group C (Low Skill / Low Will) to reduce costs.
   - Consider layoffs for employees with high education but low performance (Prior to Layoff segment).

2. **Model Optimization:**
   - Fine-tune machine learning models to improve prediction accuracy.
   - Use balanced datasets to address class imbalance and improve model performance.

3. **Employee Training:**
   - Implement training programs to improve employee skills and performance.
   - Use the EDAC and GROW models for training new and existing employees.

## Prerequisites
- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, xgboost
