# logistic_regression_day2.py
Logistic Regression and classification
# 🤖 Logistic Regression – Day 2 of AI Engineer Journey

## 🔍 What is Logistic Regression?

Logistic Regression is a **supervised machine learning algorithm** used for **classification tasks**, especially **binary classification** (yes/no, spam/not spam, cancer/no cancer, etc.).

Instead of predicting a continuous value (like Linear Regression), it predicts **probabilities** between 0 and 1 using the **sigmoid function**, and maps those to class labels (e.g., 0 or 1).

Formula:
\[
\sigma(x) = \frac{1}{1 + e^{-x}}
\]

---

## 🔄 How is it Different from Linear Regression?

| Feature              | Linear Regression                     | Logistic Regression                          |
|----------------------|----------------------------------------|-----------------------------------------------|
| Task Type            | Regression (continuous output)         | Classification (discrete output)             |
| Output               | Real numbers                           | Probability between 0 and 1                  |
| Activation Function  | None                                   | Sigmoid                                      |
| Loss Function        | Mean Squared Error (MSE)               | Binary Cross-Entropy                         |
| Output Interpretation| Direct prediction                      | Thresholded (e.g., > 0.5 = class 1)          |

---

## 📊 Summary of My Results

- **Dataset**: Breast cancer classification (`sklearn.datasets.load_breast_cancer`)
- **Model**: Logistic Regression (`scikit-learn`)
- **Test Accuracy**: **96%**
- **Performance**:
  - Precision (Class 1): 0.95
  - Recall (Class 1): 0.99
  - F1 Score (Class 1): 0.97

### 🔢 Confusion Matrix
[[39 4]
[ 1 70]]



- Only 5 incorrect predictions out of 114 samples.
- Very high precision and recall, especially for class 1 (cancer).
- Model generalizes well to unseen data.
