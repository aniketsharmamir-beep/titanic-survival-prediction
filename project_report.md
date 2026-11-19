# Titanic Survival Prediction — Project Report

## 1. Problem
Predict passenger survival (`survived`) from `raw_dataset.csv` using passenger demographics and ticket features, and identify which factors were most associated with survival.

## 2. Approach
- **Data Cleaning:** Loaded `raw_dataset.csv`, removed duplicates, selected core features, filled missing numeric values with the median and missing categorical values with the mode, and exported `data/processed/cleaned_dataset.csv`.
- **EDA:** Inspected target balance, survival rates by sex and passenger class, age distribution, and numeric correlations.
- **Modeling & Evaluation:** Applied one-hot encoding, split data 80/20 with stratification (`random_state=42`), and compared **Logistic Regression** (baseline) against **Random Forest** using Accuracy, Precision, Recall, and F1-Score.

## 3. Results
| Model | Accuracy | Precision | Recall | F1-Score |
| --- | --- | --- | --- | --- |
| Logistic Regression (Baseline) | *(paste from Cell 4)* | *(paste)* | *(paste)* | *(paste)* |
| Random Forest | *(paste from Cell 4)* | *(paste)* | *(paste)* | *(paste)* |

## 4. Insights & Limitations
- **Key Insights:** Sex, ticket class (`pclass`), and fare strongly relate to survival rates.
- **Limitations & Next Steps:** Limited set of engineered features; cross-validation and hyperparameter tuning are good next steps.
