# Employee Attrition Prediction

## Overview
Employee attrition is a critical issue in Human Resource Management. This project uses machine learning techniques to predict whether an employee is likely to leave a company based on various features such as job satisfaction, age, department, and more.

This project aims to build an accurate predictive model using real-world employee data and provide actionable insights that can help organizations proactively manage retention.

## Objectives
- Analyze employee-related features and their impact on attrition.
- Preprocess and clean the data to prepare it for modeling.
- Train and evaluate classification models to predict attrition.
- Identify the most influential features contributing to employee turnover.

## Dataset
- **Source**: IBM HR Analytics Employee Attrition & Performance dataset.
- **Size**: ~35 features for ~1,470 employees.
- **Target Variable**: `Attrition` (Yes/No)

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

## Workflow

### 1. Data Preprocessing
- Removed unnecessary columns (e.g., `EmployeeCount`, `Over18`).
- Converted categorical variables using Label Encoding.
- Checked for missing values and outliers.

### 2. Exploratory Data Analysis (EDA)
- Visualized attrition across various features like:
  - Age groups
  - Job roles
  - Monthly income
  - Work-life balance
- Identified patterns and correlations using heatmaps.

### 3. Feature Selection
- Removed constant/irrelevant features.
- Evaluated feature importance using tree-based models.

### 4. Model Building
- **Algorithms Tried**:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Gradient Boosting
- **Evaluation Metrics**:
  - Accuracy
  - Precision, Recall
  - F1 Score
  - ROC-AUC

### 5. Final Model
- **Best Performing Model**: Random Forest Classifier  
- **Accuracy**: ~87%  
- **ROC-AUC**: ~0.91

## Key Insights
- Employees with low job satisfaction and high overtime are more likely to leave.
- Monthly income, environment satisfaction, and years at the company are strong predictors.
- HR teams can focus retention efforts on specific age groups and job roles.

## Project Structure
```bash
Employee-Attrition-Prediction/
│
├── G3_Project_Employee_Attrition_Project_Final.ipynb  # Main notebook
├── README.md                                          # Project overview
└── data/                                              # (if applicable)
```

## Future Work
- Implement SMOTE for better class balance.
- Try advanced models like XGBoost or LightGBM.
- Integrate with a Flask API for live predictions.

## Author
- Sherin K Aby  
(Master’s in Management Information Systems, Drexel University)
