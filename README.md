dataset source:: https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008

# Predicting Hospital Readmission of Diabetic Patients using Data Mining

## Project Overview

This project applies data mining techniques to predict the hospital readmission rate of diabetic patients. The primary goal is to assist hospitals in improving diabetic patient care and reducing costly readmissions. The dataset used includes over 100,000 records from diabetic patient encounters between 1999 and 2008 across 130 U.S. hospitals.

We implemented three predictive models:
- Logistic Regression
- Decision Tree
- Random Forest

**Random Forest** delivered the best results with **94% accuracy**, **98% precision**, and **90% recall**.

---

## Dataset Description

- Source: Public repository on diabetic patient readmissions
- Records: 101,766 patient encounters
- Features: 50 attributes including:
  - Patient demographics
  - Medical history and diagnosis codes
  - Drug prescriptions and dosage changes
  - Lab results and hospital utilization details
  - Readmission status: `<30` (within 30 days), `>30` (after 30 days), or `No`

---

## Data Preprocessing

Key steps included:
- **Data Cleaning**: Dropped columns with >90% missing values and removed rows with critical missing data.
- **Feature Aggregation**: Grouped categorical variables like admission/discharge types.
- **Data Reduction**: Removed uninformative or redundant features.
- **Encoding & Normalization**: Converted string values to numerical, normalized age ranges, grouped lab results.
- **Target Transformation**: Converted readmission status into binary classes (`0 = No or >30 days`, `1 = <30 days`).

---

## Data Mining Techniques

| Model              | Accuracy | Precision | Recall |
|-------------------|----------|-----------|--------|
| Logistic Regression | 62%      | 64%       | 55%    |
| Decision Tree       | 90%      | 93%       | 91%    |
| **Random Forest**   | **94%**  | **98%**   | **90%**|

> **Conclusion:** Tree-based models, especially Random Forest, outperformed other models in predicting diabetic patient readmissions.

---

## Key Findings

- Patients **not monitored for A1C levels** had higher readmission rates.
- Prescription of **diabetic medications** correlated with higher readmissions.
- Some **demographic trends** appeared but did not significantly affect prediction.

---

## Future Work

- Incorporate more recent and complete datasets.
- Generalize the model to support **other medical conditions**.
- Explore **deep learning** methods for improved prediction performance.

---

## Team Contributions

| Name              | Contributions |
|-------------------|----------------|
| **Nayana Ann Moni** | Data preprocessing, logistic regression, visualization, report writing |
| **Rosmi** | Data cleaning, mining, visualizations, report writing (discussion, intro & conclusion) |
| **Adewale Arogbonlo** | Decision tree modeling, result analysis, business scenario writing |

---

References

- Clark et al. (2016). *Endoscopy International Open*
- Jiang et al. (2018). *Knowledge-Based Systems*
- Cui et al. (2018). *Elsevier*
- Goudjerkan & Jayabalan (2019). *SAI Organization*
