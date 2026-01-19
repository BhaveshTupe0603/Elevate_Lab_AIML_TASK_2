# 🧹 Complete Elevate Lab Task 2: AIML Internship

**Internship Task:** Data Cleaning & Missing Value Handling
**Intern Name:** Bhavesh
**Language:** Python (Pandas, NumPy)
**IDE:** Jupyter Notebook / Google Colab

---

## 📌 Project Overview
This project focuses on **Data Preprocessing**, specifically handling missing values and cleaning raw data. The goal is to transform a "dirty" dataset into a clean, structured format suitable for machine learning or analysis.

**Datasets Used:**
* House Prices Dataset (Primary)
* Medical Appointment No Shows (Secondary Reference)

## 🛠️ Tech Stack
* **Python:** Core programming language.
* **Pandas:** For data manipulation and DataFrame operations.
* **NumPy:** For numerical operations (handling `NaN`).
* **Seaborn/Matplotlib:** For visualizing missing data patterns (Heatmaps).

---

## 🚀 Key Features & Steps

### 1. Data Loading & Inspection
* Loaded raw data using `pd.read_csv()`.
* Identified missing values using `.isnull().sum()`.
* **Visualization:** Created a heatmap to visually locate gaps in the data.

### 2. Missing Value Imputation
* **Numerical Columns (`Price`, `LotArea`):** Filled missing values using the **Median** to avoid skewing data with outliers.
* **Categorical Columns (`BuildingType`):** Filled missing values using the **Mode** (most frequent category).

### 3. Data Cleaning
* **Column Removal:** Dropped the `Alley` column because >50% of the data was missing, making it unreliable for imputation.
* **Sanity Check:** Validated that the final dataset contains 0 null values.

---

## 📊 Results: Before vs. After

| Metric | Original Data | Cleaned Data |
| :--- | :--- | :--- |
| **Rows** | 10 | 10 |
| **Columns** | 5 | 4 |
| **Missing Values** | 13 | 0 |
| **Completeness** | 74% | 100% |

> **Note:** The `Alley` column was removed during cleaning.

---

**Author:** Bhavesh
