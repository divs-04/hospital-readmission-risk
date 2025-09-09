# Predicting Hospital Readmissions: From General Population to Diabetic-Specific Risk Modeling

## Overview

This project leverages advanced data science and machine learning techniques to predict 30-day hospital readmissions. It is divided into two phases:

- **Phase I:** Predicting readmission risk for all hospital patients.
- **Phase II:** Focused modeling for diabetic patients, a high-risk subgroup.

The notebook guides you through data exploration, feature engineering, model building, evaluation, and interpretation, with a strong emphasis on clinical relevance and actionable insights.

---

## Dataset

- **Source:** Hospital admissions data for 8,429 patients
- **Features:** Demographics, clinical metrics (blood pressure, cholesterol, BMI), hospitalization details, chronic disease indicators, treatment plans, and readmission outcome.

---

## Key Steps

1. **Data Exploration & Cleaning**
   - Summary statistics, missing value analysis, and structural fixes (e.g., splitting blood pressure into systolic/diastolic).
2. **Feature Engineering**
   - Creation of interaction features (e.g., age × disease burden, BMI ratio, glycemic risk score).
3. **Imputation & Encoding**
   - Median/mode imputation, categorical encoding (One-Hot, Ordinal, Label).
4. **Modeling**
   - Baseline models: Logistic Regression, SVC, Decision Tree, Random Forest.
   - Class balancing, hyperparameter tuning, threshold optimization.
5. **Evaluation**
   - Precision, recall, F1 score, confusion matrix, feature importance.
6. **Interpretation**
   - Clinical insights, actionable findings, and recommendations for hospital management.

---

## Results

- **Best Model:** Random Forest with custom thresholding for high recall.
- **General Population:** Key predictors include BMI ratio, age burden, blood pressure × cholesterol, and discharge destination.
- **Diabetic Patients:** Cardiovascular risk (BP × cholesterol), BMI, disease burden, and age × A1C interaction are most influential.

---

## How to Run

1. **Requirements**
   - Python 3.8+
   - pandas, numpy, matplotlib, seaborn, scikit-learn

2. **Usage**
   - Open `hosptial_readm_pred.ipynb` in Jupyter or VS Code.
   - Run cells sequentially for full analysis and modeling workflow.

---

## Visuals

- Distribution plots, correlation heatmaps, confusion matrices, and feature importance charts are included for clear interpretation.

---

## References

- [Cleveland Clinic: Cholesterol & BMI Guidelines](https://my.clevelandclinic.org/health/articles/11920-cholesterol-numbers-what-do-they-mean)
- [BMC Medical Informatics: Diabetes Readmission Study](https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/s12911-021-01423-y?utm_source=chatgpt.com#Sec2)

---

## Author

**Divyanshu Srivastava**

---

## License

This project is for educational and research purposes. Please cite appropriately if used in publications.

---

## Contact

For questions or collaboration, please reach out via GitHub or email.
