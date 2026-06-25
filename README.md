# Advanced EDA & Feature Engineering

## Project Overview

This project demonstrates enterprise-grade data preprocessing and feature engineering techniques on an e-commerce dataset.

The goal is to transform raw transactional data into a clean, machine-learning-ready dataset through:

- Missing value handling
- Outlier detection and treatment
- Statistical analysis
- Feature engineering

---

## Dataset Information

Rows: 1200

Columns:

- OrderID
- Date
- CustomerID
- Product
- Quantity
- UnitPrice
- ShippingAddress
- PaymentMethod
- OrderStatus
- TrackingNumber
- ItemsInCart
- CouponCode
- ReferralSource
- TotalPrice

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- SciPy
- Matplotlib
- Seaborn

---

## Project Pipeline

### 1. Data Loading

Load raw Excel dataset.

### 2. Exploratory Data Analysis

- Summary statistics
- Missing value analysis
- Correlation analysis
- Distribution analysis

### 3. Missing Value Treatment

Methods implemented:

- Mean Imputation
- Median Imputation
- KNN Imputation

### 4. Outlier Detection

Methods implemented:

- Z-Score Method
- Interquartile Range (IQR)

### 5. Feature Engineering

New features created:

1. OrderMonth
2. OrderYear
3. AvgItemValue
4. CartEfficiency
5. UsedCoupon

### 6. Export

Generate a clean dataset ready for machine learning.

---

## Results

### Missing Values

| Column | Missing |
|---------|---------|
| CouponCode | 309 |

### Features Created

| Feature | Description |
|----------------|-------------------------------|
| OrderMonth     |     Month extracted from date |
| OrderYear      |     Year extracted from date  |
| AvgItemValue   |     TotalPrice / Quantity     |
| CartEfficiency |     Quantity / ItemsInCart    |
| UsedCoupon     |     Binary coupon indicator   |

## Output:

```text
cleaned_feature_engineered_dataset.csv
```