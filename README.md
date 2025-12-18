# Retail Sales Data Analysis using NumPy

## 📌 Project Overview
This project demonstrates a real-world data analysis pipeline using **NumPy only**.
The goal is to clean, analyze, and normalize a large retail sales dataset while
handling common data quality issues such as missing values, invalid entries, and outliers.

The project is designed to showcase **practical NumPy skills** suitable for data
analysis and machine learning preprocessing.

---

## 📊 Dataset Description
- **Rows:** 365 (Daily sales for one year)
- **Columns:** 8 (Products A–H)
- **Data Issues Included:**
  - Missing values (`NaN`)
  - Invalid values (negative sales)
  - Extreme outliers
  - Natural sales variation

The dataset was synthetically generated to closely resemble real retail sales data.

---

## 🛠️ Tools & Technologies
- Python
- NumPy

---

## 🔍 Data Processing Steps

### 1️⃣ Data Inspection
- Checked array shape, size, dimensions, and data types
- Counted missing values

### 2️⃣ Missing Value Handling
- Replaced missing values using **column-wise mean imputation**

### 3️⃣ Invalid Data Removal
- Removed rows containing negative sales values

### 4️⃣ Outlier Detection & Removal
- Used **Robust Z-Score Method**:
  - Median and Median Absolute Deviation (MAD)
  - Outliers defined as |robust_z| > 3.5
- Removed rows containing any outlier

### 5️⃣ Business Metrics
- Total yearly sales per product
- Average daily sales per product
- Identified the best-performing product

### 6️⃣ Data Normalization
- Applied **Min–Max scaling** (column-wise)
- Prepared data for machine learning models

---

## 📈 Key Outcomes
- Cleaned and validated sales dataset
- Robust handling of outliers
- Business insights derived from raw data
- ML-ready normalized dataset
