# 🏢 Employee Distribution & Labor Rights: A Statistical Perspective

This repository contains a deep-dive statistical analysis of employee satisfaction, demographics, and the factors leading to turnover (attrition). Developed as a core project for a 2024/2025 statistics course, the study focuses on how company management strategies impact worker longevity.

## 🚀 Project Overview
The "Strategy of Management" is a critical factor in a firm's profitability and stability. Our research specifically investigates which variables most influence an employee's decision to leave.

### 📊 The Dataset
Since real-world HR data is often private, our team curated a **custom dataset** (150 rows, 20 columns) by synthesizing information from Kaggle, HR forums, and social media surveys. It reflects a realistic representation of a modern company.

**Key features analyzed:**
* **Demographics:** Age, Gender, Marital Status, Education.
* **Workplace Factors:** Department, Job Role, Monthly Salary, Distance from Home.
* **Performance & Growth:** Years at Company, Training Frequency, Time since Last Promotion.
* **Subjective Ratings:** Environment Satisfaction, Job Satisfaction, Performance Rating.

---

## 🛠 Tech Stack
* **Language:** Python
* **Environment:** Google Colab / Jupyter
* **Libraries:**
    * `Pandas` & `NumPy`: Data processing.
    * `Matplotlib`, `Seaborn`, `Plotly`: Interactive and static visualizations (Violin plots, Histograms, Boxplots).
    * `Scipy.stats`: Statistical testing (Chi-square, K-S, Shapiro-Wilk).
    * `Statsmodels`: Linear regression modeling.
    * `PrettyTable`: Organized console reporting.

---

## 📋 Key Research & Analysis

### 1. Descriptive Statistics
We analyzed the "Mean, Median, and Mode" of variables like **Age (Avg: 36.3)** and **Distance from Home (Avg: 9.2km)** to determine if basic logistics or demographics drive attrition.

### 2. Hypothesis Testing (Chi-Square)
We tested dependencies between categorical variables with a significance level of **α = 0.05**:
* **Marital Status vs. Business Travel:** Result: *Independent* (p=0.71).
* **Gender vs. Attrition:** Result: *Independent* (p=0.67).
* **Education Field vs. Department:** Result: **Dependent** (p=0.0) — showing a strong link between specific degrees and department placement.

### 3. Normality Testing & Distributions
To determine if our data follows a Normal Distribution, we employed:
* **Kolmogorov-Smirnov (K-S) & Shapiro-Wilk Tests**
* **QQ-Plots** for visual verification of variables like Salary, Age, and Training levels.

### 4. Advanced Modeling
* **Confidence Intervals:** Estimation of mean values for numerical variables and proportions for categorical ones.
* **Linear Regression:** A bonus model created to predict trends in employee behavior based on the analyzed features.

---

## 💡 Key Findings
* **The "Monotony" Theory:** Employees with long tenures but low travel frequency/promotions showed higher attrition rates.
* **The Distance Factor:** Even a distance of 10km (round trip) was a statistically significant reason for leaving, suggesting a demand for remote work.
* **Education Impact:** Highly specialized technical staff reported lower environment satisfaction, indicating challenges in integrating technical talent into traditional corporate cultures.

---

## 📂 Project Structure
* `employeeSatisfactionAnalysis.ipynb`: The main Google Colab notebook.
* `custom_dataset.csv`: The synthesized dataset used for analysis.
