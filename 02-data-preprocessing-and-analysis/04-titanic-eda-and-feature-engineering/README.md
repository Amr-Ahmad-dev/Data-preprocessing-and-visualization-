# 🚢 Titanic Survival Analysis: End-to-End EDA & Feature Engineering

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Dataset](https://img.shields.io/badge/Dataset-Titanic-red.svg)](#)
[![Workflow](https://img.shields.io/badge/Workflow-End--to--End%20EDA-success.svg)](#)
[![Significance](https://img.shields.io/badge/Significance-Top%20Tier%20Project-gold.svg)](#)

## 📌 Project Overview
An end-to-end applied data science project analyzing passenger survival patterns from the 1912 Titanic shipwreck. This project demonstrates production-grade exploratory data analysis (EDA), data imputation, feature engineering, and statistical narrative building.

---

## 🛠️ Pipeline Architecture

### 1. Data Ingestion & Integrity Audit
- Ingestion of Seaborn's canonical Titanic dataset (891 passenger records, 15 attributes).
- Auditing missing value prevalence across `age`, `embarked`, `deck`, and `embark_town`.

### 2. Statistical Data Cleaning
- **Age Imputation**: Filled missing values using median age across the cohort to mitigate skewness.
- **Embarked Imputation**: Imputed missing boarding ports using categorical mode (`'S'`).
- **Deck Feature Treatment**: Dropped the `deck` feature due to >75% missingness.
- **Record Sanitization**: Removed remaining sparse records with missing target attributes.

### 3. Comprehensive Visual EDA
- **Univariate**: Age distribution with KDE overlay, fare distribution.
- **Bivariate**: Survival rates grouped by `sex`, `pclass`, and `embark_town`.
- **Multivariate**: Fare distribution across passenger classes via box plots; age distribution by class via violin plots.
- **Collinearity**: Correlation matrix heatmap evaluating numerical relationships.

### 4. Feature Engineering
- Created `family_size = sibsp + parch + 1` to model traveling party scale.
- Evaluated survival advantages of traveling alone versus with family units.

---

## 📊 Summary of Insights
| Driver | Finding | Impact on Survival |
|---|---|---|
| **Gender** | Female survival was ~74%, Male ~19% | Primary survival predictor |
| **Class** | 1st Class (~63%) > 2nd Class (~47%) > 3rd Class (~24%) | Severe socio-economic disparity |
| **Family Size** | Parties of 2–4 had highest survival | Moderately sized groups assisted each other |
| **Fare** | Higher fare correlated with upper decks and lifeboats | Strong positive survival correlation |

---

## 💻 Code Structure
- **Notebook**: [`titanic_eda_and_feature_engineering.ipynb`](./titanic_eda_and_feature_engineering.ipynb)
- **Cell Count**: 55 cells (24 code cells, 31 markdown cells)
- **Dependencies**: `pandas`, `numpy`, `matplotlib`, `seaborn`

---

## 🚀 How to Run
```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook titanic_eda_and_feature_engineering.ipynb
```
