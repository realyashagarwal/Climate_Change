# 📊 Data Preparation Notebook

This repository contains a Jupyter Notebook for preparing and transforming raw data for analysis or modeling tasks.

---

## 🧱 File Overview

- **`1_data_preparation.ipynb`**  
  A step-by-step notebook that performs the following:
  - Selects and extracts relevant features
  - Cleans and reshapes the data using `pandas`
  - Merges datasets into a unified format suitable for further analysis

---

## ⚙️ Requirements

- Python 3.7+
- Jupyter Notebook
- Dependencies:
  ```bash
  pip install pandas numpy
  ```

---

## 📂 Data Structure

The notebook expects a data file with the following structure:

| Country code | Series name | 2000 | 2001 | ... | 2020 |
|--------------|-------------|------|------|-----|------|
| USA          | GDP         | ...  | ...  | ... | ...  |
| IND          | Inflation   | ...  | ...  | ... | ...  |

It reshapes this into a long format with `country`, `year`, and feature columns.

---

## 🧠 Key Logic

- Uses `melt()` to transform year columns into rows
- Filters and maps multiple selected features
- Merges all feature dataframes using `functools.reduce`

---

## 📌 Output

A single `pandas.DataFrame` containing:
- One row per country/year
- One column per selected feature

---

## 📄 License

Feel free to use and modify for academic or personal projects.
