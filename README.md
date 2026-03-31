# Exploratory-Data-Analysis-EDA-
# Week 5: Learner Performance Analysis

## Overview
This project performs an exploratory data analysis (EDA) of student performance to identify patterns that can inform interventions for the next term. The analysis covers descriptive statistics, distributions, correlations, and group-level insights.

The dataset contains student information, study habits, attendance, quiz scores, and final scores.

---

## Dataset
**Filename:** `Week-5-Student-Scores.csv`  
**Columns:**
- `Student_ID` – Unique identifier for each student
- `Gender` – Male or Female
- `Subject` – English, Maths, or Science
- `Study_Hours_per_Week` – Average study hours per week
- `Attendance_Rate` – Proportion of classes attended (0–1)
- `Previous_Score` – Score from the previous assessment
- `Quiz1`, `Quiz2`, `Quiz3` – Scores in three quizzes
- `Final_Score` – Final assessment score

---

## Analysis Steps

### Q1 — Data Readiness & Quality Checks
- Loaded the CSV into a pandas DataFrame.
- Checked the shape, column types, missing values, and duplicate rows.
- **Decisions:**
  - Filled missing numeric values with median to retain records.
  - Dropped duplicate rows.
  - Kept categorical columns as-is.

### Q2 — Descriptive Statistics & Distributions
- Computed summary statistics: mean, median, standard deviation, min, max, percentiles.
- Visualized `Final_Score`, `Study_Hours_per_Week`, and `Attendance_Rate` using histograms.
- **Insights:**
  - Final scores show left skew (some low performers).
  - Study hours vary widely.
  - Attendance is mostly high, with a few low cases.

### Q3 — Correlations & Group Analysis
- Computed correlation matrix for numeric variables.
- Plotted scatterplots of:
  - Study Hours vs Final Score
  - Attendance Rate vs Final Score
- Conducted cross-tab analysis of average `Final_Score` by `Subject` and `Gender`.
- **Insights:**
  - Higher study hours and attendance correlate with better final scores.
  - Maths and Science students generally perform slightly better.
  - Gender differences are minor.

---

## Requirements
- Python 3.x
- Libraries:
  - `pandas`
  - `matplotlib`
  
> Note: This notebook does not require seaborn to run.

---

## How to Run
1. Clone the repository or download the files.
2. Ensure `Week-5-Student-Scores.csv` is in the same directory as the notebook.
3. Open the Jupyter Notebook.
4. Run all cells sequentially.
5. Review the plots, tables, and markdown insights for submission.

---

## Author
Maphuti – Week 5 Assessment Submission

---

## Deliverables
1. Jupyter Notebook: `Week5_Learner_Performance_EDA.ipynb`
2. Dataset: `Week-5-Student-Scores.csv`
3. README: `README.md`
