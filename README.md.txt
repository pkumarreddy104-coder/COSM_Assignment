# Student Performance Statistical Tests

This project performs statistical hypothesis testing using the **StudentsPerformance** dataset from Kaggle.  
We compare **Math Score** and **Reading Score** using:

- Z-Test
- T-Test
- F-Test

## 📂 Dataset
Dataset used: **StudentsPerformance.csv**

---

## 📊 Statistical Tests

### 🟡 T-Test
Compares the means of two samples (Math vs Reading).

### 🔵 Z-Test
Very similar to T-test when sample size is large.

### 🔴 F-Test
Compares the variances between the two scores.

## 📦 Requirements

Install the following packages:
pip install pandas numpy scipy statsmodels matplotlib

## ▶️ How to Run

Run the Python script:

python main.py

## 📈 Results Interpretation

Use the P-value:

- **P-value < 0.05** → Reject the null hypothesis  
  ✔ There is a significant difference between the scores.

- **P-value ≥ 0.05** → Fail to reject the null hypothesis  
  ✔ No significant difference.

## ✔️ Example Output
T-test: statistic = -4.627, p-value = 3.94e-06
Z-test: statistic = -4.627, p-value = 3.70e-06
F-test: statistic = 1.078

These results show a **statistically significant difference** between Math and Reading scores.
## 👨‍🏫 Submitted By
Name:K.PREM KUMAR REDDY
Roll No:24XV1M6753
Course:CSE-DS








