# 🐼 Data Wrangling & Manipulation with Pandas

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Library](https://img.shields.io/badge/Library-Pandas-150458.svg)](https://pandas.pydata.org/)
[![Topic](https://img.shields.io/badge/Topic-Tabular%20Wrangling-informational.svg)](#)

## 📌 Project Overview
This project provides an exhaustive exploration of Pandas DataFrames and Series. It serves as an essential manual for transforming raw, unorganized tabular data into pristine datasets ready for statistical modeling and exploratory analysis.

---

## 🛠️ Data Pipeline Lifecycle Covered
```
Raw Data Ingestion ➔ Structural Audit ➔ Conditional Slicing ➔ Cleaning & Imputation ➔ Grouped Aggregations
(pd.DataFrame)       (info, describe)    (.loc / .iloc)         (dropna, fillna)          (groupby, agg)
```

### 1. Data Structures & Inspection
- Difference between 1D `pd.Series` and 2D `pd.DataFrame`.
- Memory usage profiling, data type detection, and summary statistics (`describe()`).

### 2. Precise Querying & Filtering
- Explicit label indexing (`.loc`) vs integer coordinate indexing (`.iloc`).
- Compound Boolean masks using `&`, `|`, and `~`.

### 3. Missing Data Treatment
- Null detection (`isna().sum()`).
- Systematic dropping vs imputation techniques (`fillna()`).

### 4. GroupBy & Analytical Reporting
- Grouping by single and multi-level categorical factors.
- Custom aggregation pipelines (`.agg({'col1': 'mean', 'col2': 'sum'})`).

---

## 💻 Code Structure
- **Notebook**: [`pandas_data_manipulation.ipynb`](./pandas_data_manipulation.ipynb)
- **Cell Count**: 61 cells (27 code cells, 34 markdown cells)
- **Dependencies**: `pandas`

---

## 🚀 How to Run
```bash
pip install pandas
jupyter notebook pandas_data_manipulation.ipynb
```
