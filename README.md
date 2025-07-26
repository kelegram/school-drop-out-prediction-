# 🎓 Student Dropout Prediction (Machine Learning Project)

This project builds a binary classification model to predict student dropout behavior using a Random Forest Classifier. The model is trained with optimized hyperparameters via GridSearchCV and includes a preprocessing step using `StandardScaler`.



---

## ✅ Objective

The main goal is to identify students likely to drop out (class `1`) versus those who are not (class `0`), using demographic and academic-related features.

---

## 🛠️ Tools & Libraries Used

- Python
- Jupyter Notebook
- Pandas, NumPy
- Scikit-learn
  - RandomForestClassifier
  - StandardScaler
  - GridSearchCV
  - Classification report
  - Confusion matrix

---

## 🧪 Model Pipeline

1. **Preprocessing:**
   - Applied `StandardScaler` to scale numerical features.

2. **Model:**
   - Trained a `RandomForestClassifier`.
   - Performed hyperparameter tuning using `GridSearchCV` with 4-fold cross-validation.


```python


Performance Metrics:
overall accuracy is 0.85
ss | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.87      | 0.87   | 0.87     | 569     |
| 1     | 0.77      | 0.77   | 0.77     | 316     |

confusion matrix 
497  72
74 242
True Negative (TN = 497) These are students who didn’t drop out and the model correctly predicted they wouldn’t.
False Positive (FP = 72) These are students who didn’t drop out, but the model incorrectly predicted they would.
False Negative (FN = 74) These are students who actually dropped out, but the model missed them.
True Positive (TP = 242) These are students who did drop out, and the model correctly predicted that.


