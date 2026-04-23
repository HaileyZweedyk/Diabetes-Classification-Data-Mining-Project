# Diabetes Classification Project


## Executive Overview

This project analyzes key health factors associated with diabetes using a dataset of 100,000 patient records. The goal is to identify the most influential predictors of diabetes and support accurate classification through machine learning models.

The results highlight HbA1c levels and blood glucose levels as the strongest indicators of diabetes, showing a clear and consistent relationship with positive diagnoses. Additional factors such as age, BMI, hypertension, and smoking history also contribute to increased risk, though to a lesser extent.

Overall, the analysis demonstrates that diabetes classification is primarily driven by glucose-related measures, with other health and lifestyle factors providing supporting context in predicting risk.

## Technologies Used

Python (NumPy, Pandas, scikit-learn, Matplotlib, Seaborn) 

## How to Run

This project can be run in Google Colab by opening the notebook and executing each cell sequentially from top to bottom.

Tableau

## Dataset and Problem Defintion

For this project, a dataset of 100,000 patients' medical records was used to predict if a patient had been diagnosed with diabetes or not. The objective of this classification was to identify key medical factors associated with the development and diagnosis of diabetes and use them to build an accurate predictive model using Decision Trees and AdaBoost. Medical factors in the dataset include: Smoking History, HbA1c Level, BMI, Blood Glucose Level, Heart Disease, Hypertension, Age, and Gender. 

## EDA


**Figure 1**

*Data Evaluation and Analysis*

![Data Evaluation and Analysis](Images/PythonDiabetesAnalysis.png)


Exploratory analysis identified strong relationships between diabetes diagnoses and elevated HbA1c, blood glucose levels, and BMI. Age trends showed increasing diagnosis rates beginning around 35, with peaks between ages 60–70.

## Model Evaluation

**Figure 2**

*Model Comparison with Confusion Matrices and Model Evaluation Metrics Table*

![Model Comparison with Confusion Matrices](Images/ModelComparison.png)

![Model Evaluation Metrics](Images/ModelEval.png)

Three models were evaluated: Decision Tree, AdaBoost, and Random Forest.

- **Decision Tree** achieved the highest precision (100%) but lower recall, indicating missed positive cases.
- **AdaBoost** achieved the highest recall, making it more effective for identifying diabetic patients.
- **Random Forest** provided the most balanced performance across all metrics.

Due to the importance of minimizing missed diagnoses in medical classification, AdaBoost was selected as the most appropriate model.

## Feature Importance

**Figure 3**

*AdaBoost Importance Values*

![AdaBoost Feature Importance](Images/AdaBoostImportance.png)

**Figure 4**

*Random Forest Importance Values*

![Random Forest Feature Importance](Images/RandomForestImportance.png)

Feature importance confirms that HbA1c and blood glucose levels are the most influential predictors.

## Tableau Dashboard

![Dashboard Preview](Images/Dashboard.png)

[Download Tableau Workbook](files/dashboard.twb)


## Key Insights

- HbA1c and blood glucose levels are the most significant predictors of diabetes.
- Risk increases with age, particularly after 30–40 years.
- BMI contributes as an additional risk factor.
- Class imbalance (90.6% non-diabetic) impacts model performance, particularly recall.

## Conclusion and Future Work

The findings confirm that glucose-related measures are the primary indicators of diabetes, with additional contributions from age and BMI.

Future improvements include addressing class imbalance through resampling techniques to improve detection of diabetic cases and reduce missed diagnoses.

