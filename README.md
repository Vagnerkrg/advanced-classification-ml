# 📊 Advanced Classification ML

Projeto de Machine Learning aplicado à previsão de churn de clientes (Customer Churn Prediction), utilizando diferentes abordagens de classificação e evolução progressiva de modelos.

---

## 🎯 Problema de Negócio

Empresas de telecomunicações enfrentam altos custos relacionados à perda de clientes (churn).

O objetivo deste projeto é prever quais clientes têm maior probabilidade de cancelar o serviço, permitindo ações preventivas de retenção e redução de churn.

---

## 🧠 Objetivo do Projeto

Construir um pipeline completo de Machine Learning para classificação de churn, comparando diferentes abordagens:

- Modelos tradicionais de Machine Learning
- Métodos ensemble
- Boosting com XGBoost
- Abordagem semi-supervisionada

O projeto é desenvolvido de forma incremental, simulando evolução de um sistema real em produção.

---

## 📁 Dataset

- Telco Customer Churn Dataset
- Problema: classificação binária
- Target:
  - 0 → Cliente permanece
  - 1 → Cliente cancela serviço

---

## ⚙️ Pipeline do Projeto

✔ Carregamento e exploração inicial dos dados  
✔ Limpeza e pré-processamento  
✔ Encoding de variáveis categóricas  
✔ Separação treino/teste estratificada  
✔ Treinamento de múltiplos modelos:
  - Logistic Regression
  - Decision Tree
  - Random Forest  
✔ Implementação de pipeline com XGBoost  
✔ Avaliação de desempenho com métricas de classificação  
✔ Comparação entre modelos  

---

## 📊 Avaliação dos Modelos

Os modelos foram avaliados com:

- Accuracy
- Precision
- Recall
- F1-score

### 🏆 Melhor resultado atual:
- XGBoost (~0.799 accuracy)

---

## 🚀 Evolução do Projeto

- 🔹 Baseline de modelos tradicionais
- 🔹 Ensemble Learning (Random Forest)
- 🔹 Boosting com XGBoost
- 🔜 Semi-supervised learning (em desenvolvimento)

---

## 🧠 Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- Jupyter Notebook

---

## 📁 Estrutura do Projeto

```text
advanced-classification-ml/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_baseline_classification.ipynb
│   ├── 02_xgboost_pipeline.ipynb
│   └── 03_semi_supervised.ipynb
│
├── src/
├── models/
├── reports/
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 📌 Como executar o projeto

### Clone o repositório
```bash
git clone https://github.com/Vagnerkrg/advanced-classification-ml.git
```

### Crie o ambiente virtual
```bash
python -m venv .venv
```

### Ative o ambiente

**Windows**
```bash
.venv\Scripts\activate
```

**Mac/Linux**
```bash
source .venv/bin/activate
```

### Instale dependências
```bash
pip install -r requirements.txt
```

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