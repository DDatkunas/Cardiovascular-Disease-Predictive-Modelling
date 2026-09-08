# Cardiovascular Disease Predictive Modelling

![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/Python-3a77ad?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776ab?style=for-the-badge&logo=python&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

---

## About the Project
This project analyzes the Framingham Heart Study dataset from Kaggle to build a logistic regression model that predicts a patient's 10-year risk of developing coronary heart disease (CHD).

The goal is twofold: to explore key health drivers in the clinical data and to create an early warning system that flags high-risk patients before CHD develops.

### Preview
<img width="568" height="608" alt="image" src="https://github.com/user-attachments/assets/2c63aa80-9fa6-4dfe-86fe-02852e482ae8" />

---
## Model Performance and Key Results
- In a medical screening tool, missing a sick patient (a false negative) can be life-threatening, while mistakenly flagging a healthy patient for extra testing (a false positive) carries little practical harm. For this reason, the model prioritizes Recall — the ability to catch as many true cardiovascular cases as possible.
- Using Youden’s J-Statistic, the optimal decision threshold was set to 0.44. At this threshold, the model achieved an 80% Recall rate, successfully identifying 4 out of every 5 patients at risk of heart disease, while the overall prediction accuracy reached 59%.

---
## Repository Files
- [Analysis](https://github.com/DDatkunas/Cardiovascular-Disease-Predictive-Modelling)

---
## Limitations of the Model
- Age and Gender Bias: The model has severe performance disparities across demographic groups. It tends to over-predict risk in men over 50 (generating high false alarms) while under-predicting risk in women over 50 (missing true cases).
- Geographic Constraint: Because all patient data originates from a single town in Massachusetts, the findings may not apply directly to broader, more diverse populations.

---
## Clinical Application
- Due to these limitations, the model should not be used as a standalone diagnostic tool.
- In clinical practice, it is best suited as a preliminary triage aid—used with a lowered screening threshold for women over 50 to avoid missed cases, and paired with secondary testing for men over 50 to filter out false alarms.
