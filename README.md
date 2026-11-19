# Titanic Survival Prediction — Mini End-to-End Data Science Project

An end-to-end data science workflow built as part of my internship (Week 4 · Task 3), covering data inspection, cleaning, exploratory data analysis (EDA), baseline and ensemble modeling, evaluation, and insight reporting on the Titanic dataset (`raw_dataset.csv`).

## Project Overview

- **Problem Type:** Binary Classification (`survived`: `0` = Did Not Survive, `1` = Survived)
- **Environment:** Google Colab / Jupyter Notebook (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`)
- **Deliverables Included:**
  - End-to-end notebook (`notebooks/01_end_to_end.ipynb`)
  - Final cleaned dataset (`data/processed/cleaned_dataset.csv`)
  - Project report (`reports/project_report.md`)

## Repository Structure

- `raw_dataset.csv` — Original raw Titanic dataset
- `cleaned_dataset.csv` — Cleaned dataset ready for analysis and modeling
- `01_end_to_end.ipynb` — Complete step-by-step workflow (cleaning, EDA, modeling, evaluation)
- `rproject_report.md` — Structured summary covering Problem, Approach, Results, and Insights
- `README.md` — Project documentation and execution guide

## Workflow Steps

1. **Data Inspection & Cleaning:** Standardized column names, dropped duplicate records, handled missing values (median imputation for numeric columns and mode imputation for categorical columns), and saved the cleaned output to `data/processed/cleaned_dataset.csv`.
2. **Exploratory Data Analysis (EDA):** Examined target class distribution, survival rates across passenger sex and ticket class (`pclass`), age distributions, and feature correlations.
3. **Modeling & Evaluation:** Applied one-hot encoding to categorical features, created an 80/20 stratified train-test split (`random_state=42`), and compared a **Logistic Regression** baseline against a **Random Forest** classifier using Accuracy, Precision, Recall, and F1-Score.
4. **Report & Insights:** Summarized methodology, model performance, key takeaways, and limitations in `reports/project_report.md`.

## How to Run

1. Open `notebooks/01_end_to_end.ipynb` in **Google Colab** (or Jupyter Notebook).
2. Upload `raw_dataset.csv` when prompted in the data loading cell.
3. Run all cells from top to bottom (`Runtime` -> `Run all` in Colab) to reproduce all charts, metrics, and outputs.
