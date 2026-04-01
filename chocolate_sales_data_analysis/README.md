# 🍫 Chocolate Sales Analysis & Prediction

## Repository Name (Suggested)

**chocolate-sales-analysis-ml**

## Notebook Name (Suggested)

**chocolate_sales_eda_and_classification.ipynb**

---

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** and **Machine Learning–based classification** on a chocolate sales dataset. The goal is to understand sales patterns across countries, products, and salespersons, and to **predict whether a sale amount is High or Low** based on multiple features.

The notebook demonstrates a **complete data science workflow** including data cleaning, visualization, feature engineering, model building, and evaluation using multiple ML algorithms.

---

## 📂 Dataset Description

**File:** `Chocolate Sales.csv`

### Columns:

- **Sales Person** – Name of the salesperson
- **Country** – Country of sale
- **Product** – Chocolate product type
- **Date** – Date of transaction
- **Amount** – Sales amount (currency formatted)
- **Boxes Shipped** – Number of boxes shipped

---

## 🔍 Steps Performed in the Notebook

### 1️⃣ Data Loading & Inspection

- Loaded dataset using Pandas
- Viewed head, tail, shape, columns, and data types
- Used `info()` and `describe()` for structural and statistical overview

### 2️⃣ Data Cleaning & Preprocessing

- Converted **Amount** column from currency string to numeric
- Converted **Date** column to `datetime` format
- Extracted:
  - **Month**
  - **Year**

### 3️⃣ Exploratory Data Analysis (EDA)

- Total sales by **Country**
- Total boxes shipped by **Product**
- Total sales by **Sales Person**
- Monthly sales trends
- Scatter plot: **Boxes Shipped vs Amount**

### 4️⃣ Feature Engineering

- Created a **binary target variable**:
  - High Sale (1): Amount ≥ Median
  - Low Sale (0): Amount < Median
- Selected features:
  - Country (categorical)
  - Product (categorical)
  - Boxes Shipped (numerical)
  - Month (derived from Date)

### 5️⃣ Train–Test Split

- Split data into training and testing sets using `train_test_split`

---

## 🤖 Machine Learning Models Used

All models are implemented using **Scikit-learn Pipelines** with preprocessing:

- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machine (SVM)**
- **Decision Tree Classifier**
- **Random Forest Classifier**

### Preprocessing Techniques:

- One-Hot Encoding for categorical features
- Standard Scaling for numerical features

---

## 📊 Model Evaluation

Each model is evaluated using:

- **Accuracy Score**
- **Classification Report**

A comparison table is generated to easily identify the best-performing model.

---

## 🧠 Key Learnings

- Sales performance varies significantly by **country and product**
- Feature engineering (Month, median-based classification) improves modeling
- Ensemble models (Random Forest) generally outperform simpler models
- Pipelines ensure clean, reusable, and scalable ML workflows

---

## 📁 Recommended Repository Structure

```
chocolate-sales-analysis-ml/
│
├── chocolate_sales_eda_and_classification.ipynb
├── Chocolate Sales.csv
├── README.md
├── requirements.txt
```

---

## 📦 requirements.txt (Suggested)

```
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## 🚀 How to Run

1. Clone the repository
2. Install dependencies:
  ```bash
   pip install -r requirements.txt
  ```
3. Open the notebook:
  ```bash
   jupyter notebook chocolate_sales_eda_and_classification.ipynb
  ```

---

## ✅ Use Cases

- Beginner to intermediate **EDA practice**
- Hands-on **classification modeling** example
- Demonstration of **ML pipelines** in Scikit-learn
- Academic assignments & portfolio projects

---

## 👤 Author

**Anuj Jain**

---

⭐ If you like this project, consider giving it a star on GitHub!