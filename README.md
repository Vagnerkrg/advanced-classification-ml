
# Advanced Customer Churn Classification Pipeline

End-to-end supervised learning pipeline for customer churn prediction.

This project is developed through multiple stages:

- Ensemble models (baseline)
- XGBoost pipeline optimization
- Semi-supervised learning (Self Training)
- Model comparison and performance analysis

Goal: simulate a real-world machine learning workflow with incremental improvements and a reproducible pipeline structure.

---

## 🎯 Problem Definition

Customer churn is a critical problem for subscription-based companies, especially in the telecom sector. Retaining customers is significantly more cost-effective than acquiring new ones.

This project aims to build a predictive model capable of identifying customers with a high probability of churn, enabling proactive retention strategies.

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

Semi-supervised learning (Self Training) was evaluated but did not outperform the supervised XGBoost model, highlighting that its effectiveness depends on data distribution and labeling quality.

---

## 🧠 Key Learnings

- Ensemble methods significantly improve baseline performance
- XGBoost provides strong performance for structured tabular data
- Semi-supervised learning can be useful but is highly dependent on data quality
- Proper pipeline design is critical for reproducibility and scalability

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

```bash
git clone https://github.com/Vagnerkrg/advanced-classification-ml.git

cd advanced-classification-ml

python -m venv .venv

# Windows
.venv\Scripts\activate

# Mac/Linux
source .venv/bin/activate

pip install -r requirements.txt

### Execute os notebooks
```text
01 → baseline
02 → xgboost
03 → semi-supervisionado
```

---

## 📌 Próximos passos

- Otimização de hiperparâmetros (GridSearch / RandomSearch)
- Feature importance analysis
- Implementação completa do semi-supervisionado
- Refatoração para módulos em `src/`
- README com visualizações e gráficos

---

## 📌 Autor

**Vagner Ferreira**

Data Scientist | Machine Learning | Data Engineering  
Foco em construção de soluções de IA aplicadas a problemas reais 