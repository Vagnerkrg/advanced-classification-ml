 # 🧠 ML System v1.0 — Customer Intelligence Pipeline

## 📌 Overview

O ML System v1.0 é um pipeline completo de Machine Learning desenvolvido para prever churn de clientes e analisar padrões de comportamento utilizando aprendizado supervisionado, ensemble learning e semi-supervised learning. O projeto simula um ambiente real de produção em Data Science, cobrindo desde a engenharia de dados até a exportação e inferência do modelo treinado.

## 📊 Dataset Utilizado

O projeto utiliza o dataset Telco Customer Churn, que contém dados de clientes de uma empresa de telecomunicações.

Objetivo: prever churn (evasão de clientes)  
Variável alvo: Churn (0 = não churn, 1 = churn)

Os dados incluem informações demográficas, serviços contratados, dados financeiros e tempo de contrato.

## ⚙️ Pipeline de Dados

- Tratamento de valores ausentes  
- Encoding com OneHotEncoder  
- Transformações via ColumnTransformer  
- Separação treino/teste estratificada  
- Prevenção de data leakage  
- Pipeline consistente entre treino e inferência  
- Uso de Self-Training para semi-supervised learning  

## 🤖 Modelos Utilizados

Modelos base:
- Logistic Regression  
- Decision Tree  
- Random Forest  

Modelos avançados:
- XGBoost Classifier  
- Self-Training Classifier (Semi-Supervised Learning)  

Modelo final:
SelfTrainingClassifier com XGBoost como estimador base

## 📈 Resultados

- Accuracy final aproximada: 0.78  
- Melhora significativa em relação ao baseline  
- Redução de overfitting  
- Melhor generalização com dados parcialmente rotulados  

## 💡 Insights de Negócio

- Contratos mensais aumentam churn  
- Serviços adicionais reduzem evasão  
- Tempo de contrato é forte indicador de retenção  
- Modelos ensemble superam modelos lineares  
- Semi-supervised learning melhora desempenho geral  

## 🧪 Inferência do Modelo

```python
import joblib

model = joblib.load("models/ml_system_v1.pkl")

print("Modelo carregado com sucesso")

sample = X_test_transformed[:5]

predictions = model.predict(sample)

print(predictions)

## 💾 Estrutura do Projeto

advanced-classification-ml/
├── data/
├── notebooks/
│   └── 01_ml_system_v1.ipynb
├── models/
│   └── ml_system_v1.pkl
├── reports/
│   └── metrics_v1.json
├── requirements.txt
└── README.md

---

## 🚀 Tecnologias Utilizadas

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- XGBoost  
- Joblib  
- Jupyter Notebook  

---

## 🧠 Aprendizados

- Construção de pipeline completo de Machine Learning  
- Engenharia de features  
- Ensemble learning e boosting  
- Semi-supervised learning  
- Exportação e inferência de modelo  

---

## 📌 Status do Projeto

ML SYSTEM v1.0 — COMPLETED

✔ Classification pipeline  
✔ Ensemble models (XGBoost)  
✔ Self Training (semi-supervised)  
✔ Regression module (experimental)  
✔ Unified preprocessing pipeline  
✔ Data leakage prevention  
✔ Model exported successfully  

STATUS: FINALIZED — READY FOR NEXT MODULE  

---

## 👨‍💻 Autor 

Projeto desenvolvido como portfólio de Data Science com foco em Machine Learning aplicado em cenários reais de negócio.