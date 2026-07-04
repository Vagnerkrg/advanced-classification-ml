
# Advanced Customer Churn Classification Pipeline

End-to-end machine learning pipeline for customer churn prediction in a telecom context.

This project is developed through multiple stages, simulating a real-world machine learning workflow:

- Baseline ensemble models
- Gradient Boosting with XGBoost
- Semi-supervised learning (Self Training)
- Model comparison and performance analysis

The main goal is to build a reproducible and scalable ML pipeline that evolves incrementally, improving both technical depth and modeling performance.

---

## 🎯 Problem Definition

Customer churn is one of the most critical challenges in subscription-based businesses, especially in the telecom sector. Retaining existing customers is significantly more cost-effective than acquiring new ones.

This project aims to develop a predictive model capable of identifying customers with a high probability of churn, enabling proactive retention strategies and data-driven decision making.

---

## 📊 Dataset

- Telco Customer Churn Dataset
- Binary classification problem:
  - 0 → Customer stays
  - 1 → Customer churns

---

## ⚙️ Project Pipeline

### 1. Data Processing
- Removal of irrelevant features (e.g., customerID)
- Handling categorical variables using one-hot encoding
- Train/test split with stratification

### 2. Baseline Models (Ensemble Learning)
- Logistic Regression
- Decision Tree
- Random Forest
- Model comparison using accuracy and classification metrics

### 3. Gradient Boosting (XGBoost)
- Implementation of XGBoost classifier
- Integration into preprocessing pipeline
- Performance comparison against baseline models

### 4. Semi-Supervised Learning
- Simulation of unlabeled data
- Self Training (Pseudo Labeling)
- Iterative label propagation process
- Evaluation against supervised models

---

## 📈 Results Summary

The best performing model in this project was:

- 🏆 XGBoost Pipeline (~0.799 accuracy)

Semi-supervised learning (Self Training) showed competitive performance but did not outperform the supervised XGBoost model, highlighting that results depend heavily on data distribution and label quality.

---

## 🧠 Key Learnings

- Ensemble methods significantly improve baseline performance
- XGBoost is highly effective for structured tabular data
- Semi-supervised learning is powerful but sensitive to data quality and assumptions
- A well-designed ML pipeline improves reproducibility and scalability

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## 📁 Repository Structure

```text
advanced-classification-ml/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   └── 01_baseline_classification.ipynb
│
├── src/
├── models/
├── reports/
├── requirements.txt
├── .gitignore
└── README.md


---

## 🚀 How to Run

git clone https://github.com/Vagnerkrg/advanced-classification-ml.git

cd advanced-classification-ml

python -m venv .venv

Windows:
.venv\Scripts\activate

Mac/Linux:
source .venv/bin/activate

pip install -r requirements.txt

---

## ▶️ Execution Flow

Run the main notebook:

01_baseline_classification.ipynb

This notebook contains the full machine learning pipeline:
- data preprocessing
- baseline models
- ensemble learning
- XGBoost pipeline
- semi-supervised learning

---

## 📌 Next Steps

- Hyperparameter tuning (GridSearch / RandomSearch)
- Feature importance analysis
- Refinement of semi-supervised learning approach
- Refactoring into modular src/ structure
- Improved documentation and visualization

---

## 👨‍💻 Author

Vagner Ferreira  
Data Scientist | Machine Learning | Data Engineering  
Focused on building end-to-end AI solutions applied to real-world problems