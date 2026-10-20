# 📊 Data Preprocessing, Wrangling & Exploratory Analysis Track
[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB.svg?logo=python&logoColor=white)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/Library-NumPy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)
[![Pandas](https://img.shields.io/badge/Library-Pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Library-Matplotlib-orange.svg)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Library-Seaborn-blueviolet.svg)](https://seaborn.pydata.org/)
[![Status](https://img.shields.io/badge/Curriculum-Production%20Ready-brightgreen.svg)](#)
[![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENSE)
An end-to-end, hands-on curriculum mastering the complete **Data Preprocessing, Feature Engineering, and Statistical Visualization** lifecycle in Python. 
Raw real-world data is notoriously messy, incomplete, and unstructured. This track transitions from low-level vectorized array manipulation to high-level tabular wrangling, visual storytelling, and concludes with a full-scale clinical/historical capstone case study.
---
## 🏗️ The Data Pipeline Lifecycle
```text
                  [ DATA PREPROCESSING & EDA WORKFLOW ]
      ┌────────────────────────────────────────────────────────┐
      │        PILLAR 1: VECTORIZED TENSOR COMPUTATION         │
      │                  (NumPy Operations)                    │
      └──────────────────────────┬─────────────────────────────┘
                                 │
                                 ▼
      ┌────────────────────────────────────────────────────────┐
      │          PILLAR 2: TABULAR DATA ENGINEERING            │
      │         (Pandas Cleansing, Querying & Grouping)        │
      └──────────────────────────┬─────────────────────────────┘
                                 │
                                 ▼
      ┌────────────────────────────────────────────────────────┐
      │       PILLAR 3: STATISTICAL VISUAL STORYTELLING        │
      │            (Matplotlib & Seaborn Plots)                │
      └──────────────────────────┬─────────────────────────────┘
                                 │
                                 ▼
      ┌────────────────────────────────────────────────────────┐
      │     PILLAR 4: CAPSTONE END-TO-END CASE STUDY           │
      │     (Titanic Survival EDA & Feature Engineering)       │
      └────────────────────────────────────────────────────────┘

  

  
📚 Deep Dive: The 4 Track Projects

  
1️⃣ Project 1: Numerical Computing & Vectorization with NumPy

  

  
Notebook: numpy_numerical_computing.ipynb

  
Cell Count: 64 cells

  
Core Focus: High-performance multi-dimensional array structures and contiguous memory computing.

  
Key Topics:
  
  

  
Tensor creation: np.array(), zeros(), ones(), eye(), arange(), linspace().

  
Eliminating pure Python loops via vectorized operations and contiguous C-level memory buffers.

  
Dimension alignment using broadcasting semantics.

  
Slicing multi-dimensional grids, stride indexing, and boolean mask filtering.

  
Linear algebra primitives (dot products @, matrix transpositions) and statistical reductions (mean, std, min, max, cumsum across designated axes).

  

  

  

  
2️⃣ Project 2: Tabular Data Wrangling & Manipulation with Pandas

  

  
Notebook: pandas_data_manipulation.ipynb

  
Cell Count: 61 cells

  
Core Focus: Industrial data engineering, relational indexing, schema auditing, and aggregations.

  
Key Topics:
  
  

  
1D pd.Series vs. 2D pd.DataFrame structural internals.

  
Immediate dataset health audits: .info(), .describe(), .shape, .dtypes, and null tracking.

  
Explicit coordinate selection (.loc[] label indexing vs. .iloc[] integer positioning).

  
Robust data sanitation: Detecting missing entries (.isna()), dropping invalid rows (.dropna()), and value imputation (.fillna()).

  
Relational grouping: .groupby() pipelines paired with multi-metric aggregation dictionaries (.agg()).

  

  

  

  
3️⃣ Project 3: Statistical Data Visualization with Matplotlib & Seaborn

  

  
Notebook: data_visualization_matplotlib_seaborn.ipynb

  
Cell Count: 43 cells

  
Core Focus: Visual grammar, distribution inspection, and publication-ready multi-panel dashboards.

  
Key Topics:
  
  

  
Matplotlib Figure vs. Axes object hierarchy and multi-panel layout design (plt.subplots).

  
Continuous distribution plots: Histograms, Kernel Density Estimation (KDE), and cumulative frequencies.

  
Categorical evaluations: Bar charts, count plots, box plots (IQR, five-number summary), and violin plots.

  
Multivariate collinearity: Generating annotated Pearson correlation heatmaps with divergent color palettes (coolwarm, viridis).

  
Aesthetic customization: Themes (darkgrid, whitegrid), axis rotation, labels, legends, and aspect ratios.

  

  

  

  
4️⃣ Project 4: Titanic Survival Analysis (End-to-End Capstone)

  

  
Notebook: titanic_eda_and_feature_engineering.ipynb

  
Cell Count: 55 cells

  
Core Focus: Production-grade exploratory data analysis (EDA) and feature engineering on historical passenger records.

  
Key Highlights:
  
  

  
Data Hygiene & Imputation: Addressed severe missingness by imputing median age, mode embarkation town, and safely dropping the high-sparsity deck attribute (>75% missing).

  
Multivariate Hypothesis Testing:
  
  

  
Dissected the "Women and Children First" protocol (Female survival ~74% vs. Male ~19%).

  
Evaluated socio-economic class privileges (1st Class >60% vs. 3rd Class <25%).

  
Correlated fare pricing against survival rates via segmented box plots.

  

  
Domain Feature Engineering: Synthesized family_size = sibsp + parch + 1 and isolated solitary travelers (alone = True) to quantify traveling party survival advantages.

  

  

  

  
📊 Summary Comparison Matrix

  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
Project	Domain	Key Methods / Tools	Practical Capability Mastered
01	Array Computing	ndarray, broadcasting, @, axis stats	High-speed vectorized tensor math without Python loops
02	Tabular Wrangling	.loc, .iloc, .groupby(), .fillna()	Ingesting, cleaning, filtering, and aggregating business data
03	Statistical Plotting	plt.subplots, sns.histplot, sns.heatmap	Designing clear, publication-ready visual diagnostics
04	Applied Capstone	End-to-end EDA, Feature Engineering	Solving a real-world problem from raw data to insights

  

  
📁 Repository Directory Structure

  
text
data-preprocessing-and-visualization/
│
├── 01-numpy-numerical-computing/
│   ├── README.md
│   └── numpy_numerical_computing.ipynb
│
├── 02-pandas-data-manipulation/
│   ├── README.md
│   └── pandas_data_manipulation.ipynb
│
├── 03-data-visualization-matplotlib-seaborn/
│   ├── README.md
│   └── data_visualization_matplotlib_seaborn.ipynb
│
├── 04-titanic-eda-and-feature-engineering/
│   ├── README.md
│   └── titanic_eda_and_feature_engineering.ipynb
│
├── requirements.txt
└── README.md                                  <-- Track Master Documentation

  

  
🚀 Quickstart Guide

  
1. Clone the Track Repository

  
bash
git clone https://github.com/<your-username>/data-preprocessing-and-visualization.git
cd data-preprocessing-and-visualization

  
2. Set Up Virtual Environment & Install Dependencies

  
bash
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS / Linux:
source venv/bin/activate
pip install -r requirements.txt

  
requirements.txt

  
text
numpy>=1.22.0
pandas>=1.5.0
matplotlib>=3.6.0
seaborn>=0.12.0
scipy>=1.9.0
jupyter>=1.0.0

  
3. Launch Jupyter Notebook

  
bash
jupyter notebook

  

Navigate to any project directory and run the notebooks sequentially to follow the curriculum.


  
