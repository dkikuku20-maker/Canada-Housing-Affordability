# 🏠 Housing Affordability in Canada

## 📌 Overview
This project analyzes housing affordability in Canada using econometric modeling and machine learning.

The goal is to understand how **interest rates, income, and housing supply** affect affordability across provinces.

---

## 📊 Key Questions
- How do interest rates impact housing affordability?
- Does income growth improve affordability?
- What role does housing supply play?
- Can we predict affordability using machine learning?

---

## 🧠 Methods Used

### Econometrics
- Panel Data Regression (Fixed Effects)
- Log-linear model (ln(PIR))
- Policy simulation (interest rate, income, supply shocks)

## 🤔 Why This Approach?

### Why Panel Regression (Fixed Effects)?
Housing data varies across both **time (years)** and **regions (provinces)**.

A panel fixed-effects model was chosen because:
- It controls for **unobserved regional differences** (e.g., BC vs Quebec housing markets)
- It isolates **within-province changes over time**
- It reduces bias from missing variables that do not change over time

Alternative models like simple OLS regression were not used because they would ignore these regional effects and produce biased estimates.

---

### Why Log Transformation (ln(PIR), ln(Income))?
Log transformations were used because:
- They allow interpretation in **percentage terms**
- They reduce the impact of extreme values
- They stabilize variance in economic data

This is standard practice in econometric modeling.

---

### Why Random Forest (Machine Learning)?
Random Forest was chosen because:
- It captures **nonlinear relationships** between variables
- It handles interactions automatically (e.g., income + interest rate effects)
- It is robust to overfitting compared to single decision trees

Alternative models considered:
- Linear Regression → too simple, assumes linear relationships
- Gradient Boosting → more complex and harder to interpret

Random Forest provides a good balance between **performance and interpretability**.

---

### Why Combine Econometrics + Machine Learning?
Each method serves a different purpose:

- Econometrics → explains relationships (cause and effect)
- Machine Learning → improves prediction accuracy

Using both approaches allows the project to:
- Provide **economic interpretation**
- Deliver **predictive insights**

This combination makes the analysis more complete and practical.

### Machine Learning
- Random Forest Regressor
- Train/Test split
- Evaluation using Mean Squared Error (MSE)

---

## 📂 Data Sources
- Statistics Canada (Income data)
- Bank of Canada (Interest rates)
- CMHC (Housing supply)
- NHPI (Housing prices)

---

## 📈 Key Results
- Higher interest rates → lower affordability  
- Higher income → improved affordability  
- Strong regional differences across provinces  
- Machine learning model achieved MSE ≈ 0.008  

---

## 📊 Visualizations
(Add your plots here — screenshots or images)

---

## 🛠️ Tech Stack
- Python (Pandas, NumPy, Scikit-learn)
- Matplotlib / Seaborn
- Jupyter Notebook

---
---

## 📌 Impact
This project helps understand housing affordability using real data and can support:
- Policy analysis
- Financial risk assessment
- Housing market insights

---

## 📬 Contact
Feel free to connect with me on LinkedIn.