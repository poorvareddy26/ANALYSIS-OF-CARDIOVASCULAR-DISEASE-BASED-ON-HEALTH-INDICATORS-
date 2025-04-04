 Project Overview
This project explores the relationship between key health indicators and the presence of Cardiovascular Disease (CVD) using a health screening dataset. Cardiovascular disease is a leading cause of global mortality, and identifying associated risk factors is crucial to reducing its burden. Our aim was to analyze CVD prevalence, examine correlations between variables, and develop predictive machine learning models to detect CVD based on individual health profiles.

The study is cross-sectional in nature and seeks to provide actionable insights to improve preventive healthcare, especially for high-risk individuals.

❓ Research Questions
What are the significant health indicators associated with cardiovascular disease?

How do these indicators relate to the presence of cardiovascular disease?

Can we use machine learning models to predict the occurrence of CVD based on these variables?

Dataset
Source: Kaggle - Health Screening Dataset

Format: CSV

Contents:

Demographics: Age, Gender

Clinical Measurements: Systolic/Diastolic Blood Pressure, BMI, Cholesterol, Glucose

Lifestyle Factors: Smoking, Alcohol, Physical Activity

Target Variable: cardio (presence/absence of CVD)
 Data Cleaning & Preparation
No missing values were found in the dataset.

Columns were renamed for clarity.

Non-numeric categorical variables were identified and encoded.

Outliers were detected using box plots and scatter plots, then handled via:

Central tendency imputation

Binning

Robust statistical methods

Performed normality testing using:

Shapiro-Wilk Test

Histograms

Q-Q Plots

📈 Exploratory Data Analysis
Descriptive statistics computed post-cleaning.

Correlation matrix showed:

Moderate positive correlation between cardio and age, systolic BP, diastolic BP, BMI.

Weak but significant correlation with cholesterol and glucose.

Kendall’s Tau and Spearman’s Rho used to assess monotonic relationships.

Both tests showed statistically significant but weak correlations.

Statistical Tests
✅ Chi-Square Tests
Used to evaluate associations between categorical variables and the presence of CVD.

Found significant associations with:

Age group

Gender

Blood pressure

Cholesterol

✅ Logistic Regression
Assessed the predictive power of health indicators.

Found statistically significant relationships between:

Age

Systolic BP

Cholesterol

BMI

Smoking (weak but present)

🤖 Machine Learning Modeling
✅ Models Trained:
Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Support Vector Machine (SVM)

✅ Preprocessing:
Feature scaling

Train-test split

✅ Evaluation Metrics:
Accuracy

Precision

Recall

F1 Score

Each model was assessed using these metrics to evaluate the quality of CVD prediction.

🧠 Key Findings
Strong predictors of CVD in the dataset:

Age (50–60 years group was most affected)

Gender (males at higher risk)

Systolic Blood Pressure (≥135 mmHg)

Cholesterol (higher levels linked to CVD)

BMI (especially in the obese range 30–40)

Weak or no clear relationship observed for:

Physical activity

Alcohol consumption

Smoking (surprisingly, non-smokers showed higher CVD in this dataset)
Results:
Based of the results of the correlation analysis and hypothesis tests we have identified that the health indicators of age, gender, blood pressure, cholesterol level, and smoking are the most important risk factors for CVD in the study population. Therefore, we couldn’t accept null hypothesis.
Systolic blood pressure, Age, cholesterol, weight, BMI have strong correlation with cardiovascular disease and the attributes of glucose, smoking, alcohol, physical activity has weak correlation with cardiovascular disease.
Based on the performance metrics of machine learning models we used, the developed predictive machine learning models can predict the presence of cardiovascular disease based on these indicators.


🔚 Conclusion
This cross-sectional analysis highlights that age, systolic BP, BMI, and cholesterol are key risk indicators of cardiovascular disease. The machine learning models showed potential for predictive application, especially in screening tools. However, the study also emphasized the need for longitudinal research to establish causal pathways and the integration of more diverse data to improve model robustness.


