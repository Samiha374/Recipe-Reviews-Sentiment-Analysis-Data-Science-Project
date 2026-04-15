# 🍽️ Recipe Reviews Sentiment Analysis (Machine Learning Project)

## 📌 Project Overview
This project performs **sentiment analysis on recipe reviews** using machine learning and natural language processing (NLP). User reviews are classified into **positive, neutral, or negative** sentiment based on review text and star ratings.

The project demonstrates an **end‑to‑end machine learning pipeline**, including data cleaning, feature engineering, AutoML, and hyperparameter optimization.

---

## 📊 Dataset Description
The dataset contains:
- User review text
- Star ratings (1–5)
- Recipe names
- User metadata

### Data Cleaning Steps
- Removed unnecessary identifier columns
- Dropped rows with missing review text or ratings
- Converted star ratings into sentiment labels:
  - 1–2 stars → Negative
  - 3 stars → Neutral
  - 4–5 stars → Positive

---

## 🎯 Machine Learning Objective
**Multiclass classification** to predict review sentiment:
- Positive
- Neutral
- Negative

---

## 🔍 Feature Engineering
The model uses:
- **Numerical features** (scaled with StandardScaler)
- **Categorical feature** (`recipe_name`) using OneHotEncoder
- **Text feature** (`review text`) using TF‑IDF Vectorization

---

## ✂️ Train–Test Split
- 80% Training data
- 20% Testing data
- Stratified sampling to preserve class balance

---

## 🤖 AutoML (AutoGluon)
AutoGluon was used to:
- Automatically train and compare multiple models
- Select the best performing model
- Optimize accuracy without manual tuning

**Evaluation Metric:** Accuracy  
**Problem Type:** Multiclass Classification

---

## ⚙️ Logistic Regression + Optuna Optimization
A custom pipeline was built using:
- ColumnTransformer
- Logistic Regression
- TF‑IDF Vectorizer

### Optimized Hyperparameters
- Regularization strength (`C`)
- Maximum TF‑IDF features

Optuna was used with **cross‑validation** to find the best parameters.

---

## 📈 Model Evaluation
Evaluation was performed using:
- Accuracy score
- Precision, Recall, F1‑Score
- Confusion Matrix visualization

---

## 🧰 Tools & Libraries
- Python
- Pandas & NumPy
- Scikit‑learn
- AutoGluon
- Optuna
- Matplotlib

---

## 💡 Skills Demonstrated
- Natural Language Processing (NLP)
- Machine Learning Pipelines
- AutoML
- Hyperparameter tuning
- Data preprocessing
- Model evaluation
- GitHub documentation

---

## 🚀 How to Run the Project
1. Clone the repository
2. Install dependencies using `requirements.txt`
3. Run the notebook or Python script

---

## ✅ Status
✔️ Completed
