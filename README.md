# 🍷 Wine Quality Prediction using Machine Learning

This project builds a classification model to predict wine quality based on physicochemical attributes. It compares the performance of **Logistic Regression**, **Random Forest Classifier**, and **Support Vector Classifier (SVC)** models and tunes the SVC model to achieve the best accuracy.

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modeling and Evaluation](#modeling-and-evaluation)
- [Results](#results)

---

## 📊 Project Overview

The goal is to predict the quality of red wine using its chemical features. The target variable is the wine quality score (ranging typically from 0 to 10).

The following machine learning algorithms were applied and compared:
- Logistic Regression
- Random Forest Classifier
- Support Vector Classifier (SVC)

SVC was further optimized using GridSearchCV, resulting in the best performance.

---

## 📁 Dataset

- **Source**: UCI Machine Learning Repository
- **File**: `winequality-red.csv`
- **Features include**:
  - Fixed Acidity
  - Volatile Acidity
  - Citric Acid
  - Residual Sugar
  - Chlorides
  - Free Sulfur Dioxide
  - Total Sulfur Dioxide
  - Density
  - pH
  - Sulphates
  - Alcohol
  - Quality (target)

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 🧹 Data Preprocessing

- Checked and removed any null or missing values
- Applied `StandardScaler` to scale the data
- Encoded the target variable for classification

---

## 📈 Exploratory Data Analysis

Used Seaborn and Matplotlib for data visualization:
- Correlation heatmap
- Feature-wise bar plots and scatter plots
- Distribution of wine quality scores

---

## 🧠 Modeling and Evaluation

Three models were created and tested:

1. **Logistic Regression**
2. **Random Forest Classifier**
3. **Support Vector Classifier (SVC)**

- Models evaluated using **F1 Score** to account for class imbalance
- **GridSearchCV** was used to tune SVC hyperparameters

---

## 🏆 Results

| Model                | F1 Score |
|---------------------|----------|
| Logistic Regression | 86%      |
| Random Forest       | 87%      |
| SVC (Base)          | 88%      |
| **SVC (Tuned)**     | **90%**  |

---
