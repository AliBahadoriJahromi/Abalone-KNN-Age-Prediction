# 🐚 Abalone Age Prediction Using K-Nearest Neighbors (KNN)

## 📌 Introduction

This project focuses on predicting the **age of abalones** (a type of marine mollusk) using features such as length, diameter, height, and various weight measurements. The dataset used is the well-known [Abalone Dataset](https://archive.ics.uci.edu/dataset/1/abalone) from the UCI Machine Learning Repository.

The age of an abalone is indirectly determined by the number of **Rings**, which is a common proxy for age estimation in marine biology.

---

## 🎯 Project Goal

The objective is to:
- Implement the **K-Nearest Neighbors (KNN)** regression algorithm
- Evaluate how different values of `k` (from 1 to 10) affect the model's performance
- Measure prediction accuracy using **Root Mean Squared Error (RMSE)**
- Visualize the RMSE for each `k` value
- Provide insights on the impact of `k` on model accuracy

---

## 🧪 Dataset Overview

- **Source**: [UCI Abalone Dataset](https://archive.ics.uci.edu/dataset/1/abalone)
- **Target variable**: `Rings` (used to approximate age)
- **Ignored feature**: `Sex` (categorical), excluded for simplification
- **Input features**:
  - Length, Diameter, Height
  - Whole weight, Shucked weight, Viscera weight, Shell weight

---

## 🛠️ Methodology

1. Load and clean the dataset
2. Drop the `Sex` (categorical) column
3. Split the data:
   - **70%** for training
   - **30%** for testing
4. Train a **KNN Regressor** for `k = 1` to `k = 10`
5. Calculate **RMSE** for each value of `k` using test data
6. Plot a line graph showing RMSE vs. `k`
7. Analyze which value of `k` yields the best performance

---

## 📈 Example Output

- A plot showing RMSE for each `k`
- Numerical summary of RMSE values
- Observations about model sensitivity to `k`

---

## 🧪 Evaluation Metric

- **RMSE (Root Mean Squared Error)** is used to evaluate the difference between predicted and actual number of rings.

---