# Student Exam Score Prediction

Predicting **Exam_Score** from student behavioral and contextual factors.  
This project covers a ML workflow: data cleaning, EDA, feature analysis, modeling, and evaluation.

---

##  Workflow
<img src="IMGs/StudentPerformanceFactors%20Workflow.png" alt="Student Performance Factors Workflow" width="600">

---

## 📌 Overview
- **Goal:** Build an accurate and interpretable model to predict `Exam_Score`.
- **Data:** 6,607 rows × 20 features.
- **Target:** `Exam_Score`.

---

## Pipeline
1. **Data Cleaning**
   - Missing values handling
   - Outlier handling & final checks
   - Encoding (ordinal + one-hot → all numeric)
2. **EDA & Visualization**
   - Target / numeric distributions
   - Categorical plots (pie + count)
   - Correlation with `Exam_Score`
   - Mutual Information
3. **Modeling**
   - Train/Test split
   - Functions: visualization, evaluation, permutation importance
   - Models: Linear, Ridge, Lasso, ElasticNet, Polynomial, Random Forest, SVR
4. **Model Comparison & Conclusion**

---

## 📊 Results

| Model          | MAE   | RMSE  | R²    |
|----------------|-------|-------|-------|
| Linear         | 0.264 | 0.311 | 0.990 |
| Ridge          | 0.264 | 0.311 | 0.990 |
| Polynomial     | 0.269 | 0.317 | 0.990 |
| ElasticNet     | 0.274 | 0.323 | 0.990 |
| Lasso          | 0.277 | 0.327 | 0.989 |
| SVR            | 0.355 | 0.450 | 0.980 |
| Random Forest  | 0.841 | 1.051 | 0.889 |

**Best choice:** **Linear / Ridge** — highest R² and lowest errors with simple, interpretable models.  
**Key predictors:** `Attendance`, `Hours_Studied`.

---
