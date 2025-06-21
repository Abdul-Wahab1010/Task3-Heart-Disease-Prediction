#  Task 3: Heart Disease Prediction

This project is part of my **AI/ML Engineering Internship** at **DevelopersHub Corporation**. It aims to build a predictive model to assess the risk of heart disease using clinical data. This task emphasizes medical data understanding, classification modeling, and model evaluation.

---

## 🎯 Objective

To predict whether a person is at risk of heart disease based on health attributes using a classification algorithm.

---

## 📂 Dataset

- **Source:** [UCI Heart Disease Dataset](https://www.kaggle.com/datasets/ronitf/heart-disease-uci)
- **Records:** 303 entries
- **Features:**
  - Age, gender, chest pain type (`cp`)
  - Resting blood pressure (`trestbps`), cholesterol, fasting blood sugar
  - Resting ECG (`restecg`), max heart rate (`thalach`), exercise-induced angina
  - ST depression, slope, number of major vessels, thalassemia
- **Target:** `target` — 1 (disease), 0 (no disease)

---

## 🔧 Data Preprocessing

- Checked for missing/null values (none found)
- Converted categorical variables (e.g., `cp`, `slope`, `thal`) to numerical format
- Applied `StandardScaler` for feature scaling
- Split data into **train** and **test** sets (80/20)

---

## 📊 Exploratory Data Analysis (EDA)

- Distribution plots for numeric features
- Correlation heatmap
- Count plots for categorical variables
- Feature-target relationships visualized using Seaborn & Matplotlib

---

## 🤖 Model Building

- **Algorithm:** `Logistic Regression`
  - Lightweight and interpretable classifier
- Model trained using `scikit-learn`
- Saved model using `joblib` as:  
  - `heart_disease_model.pkl`  
  - `scaler.pkl` (for consistent input scaling)

---

## ✅ Evaluation Metrics

| Metric            | Result         |
|-------------------|----------------|
| Accuracy          | ~85%           |
| ROC AUC Score     | ~0.90          |
| Confusion Matrix  | ✔️ Visualized  |
| ROC Curve         | ✔️ Visualized  |

---

## 💡 Key Insights

- **Chest pain type**, **thalassemia**, and **max heart rate** were strong indicators.
- The model successfully generalizes across unseen data with good ROC-AUC performance.
- Logistic Regression is suitable for binary classification in healthcare diagnostics.

---

## 📁 Files Included

| File                             | Description                                 |
|----------------------------------|---------------------------------------------|
| `heart.csv`                      | Raw dataset from UCI                        |
| `heart-disease-prediction-model.ipynb` | Complete notebook with EDA and modeling     |
| `heart_disease_model.pkl`        | Trained Logistic Regression model           |
| `scaler.pkl`                     | Scaler used during training                 |
| `README.md`                      | Project documentation                       |

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/Username/Task3-Heart-Disease-Prediction.git
cd Task3-Heart-Disease-Prediction

Install required packages:
   pip install pandas numpy seaborn matplotlib scikit-learn
```
2. Install required packages:
 
 ```bash
pip install pandas numpy seaborn matplotlib scikit-learn
```

3. Run the notebook:

 ```bash
jupyter notebook house-price-prediction.ipynb
```
## 📬 Author
Abdul Wahab
GitHub: @Abdul-Wahab1010
Internship Project - DevelopersHub Corporation | June 2025

