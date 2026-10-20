# 🔢 Numerical Computing with NumPy

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Library](https://img.shields.io/badge/Library-NumPy-013243.svg)](https://numpy.org/)
[![Topic](https://img.shields.io/badge/Topic-Vectorized%20Math-lightgrey.svg)](#)

## 📌 Project Overview
This module explores high-performance numerical computing using NumPy (`numpy`). It details how contiguous memory blocks and vectorized operations provide orders-of-magnitude speedups over vanilla Python data structures.

---

## 📚 Topics Covered
1. **Array Creation & Types**:
   - `np.array()`, `np.zeros()`, `np.ones()`, `np.eye()`.
   - Sequence generation: `np.arange()`, `np.linspace()`.
   - Random sampling: `np.random.rand()`, `np.random.randn()`, seed control.
2. **Indexing & Slicing**:
   - 1D, 2D, and multi-dimensional coordinate slicing.
   - Boolean condition masking (e.g., `arr[arr > 5]`).
3. **Broadcasting & Vectorization**:
   - Element-wise arithmetic without iterative loops.
   - Dimension expansion rules and compatibility.
4. **Linear Algebra & Statistics**:
   - Matrix multiplication (`np.dot`, `@` operator).
   - Summary reductions (`mean`, `std`, `sum`, `min`, `max`, `cumsum`, `axis` parameters).
   - Array restructuring: `reshape()`, `flatten()`, `vstack()`, `hstack()`.

---

## 💻 Code Structure
- **Notebook**: [`numpy_numerical_computing.ipynb`](./numpy_numerical_computing.ipynb)
- **Cell Count**: 64 cells (31 code cells, 33 markdown cells)
- **Dependencies**: `numpy`

---

## 🚀 How to Run
```bash
pip install numpy
jupyter notebook numpy_numerical_computing.ipynb
```
