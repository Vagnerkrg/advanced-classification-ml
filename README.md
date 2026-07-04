
# Pipeline de Classificação de Churn de Clientes

Pipeline de machine learning de ponta a ponta para previsão de churn de clientes em um contexto de telecomunicações.

Este projeto é desenvolvido em múltiplas etapas, simulando um fluxo real de trabalho em machine learning:

- Modelos base com ensemble learning
- Gradiente Boosting com XGBoost
- Aprendizado semi-supervisionado (Self Training)
- Comparação de modelos e análise de performance

O objetivo principal é construir um pipeline de ML reproduzível e escalável, evoluindo de forma incremental e melhorando continuamente a profundidade técnica e a performance dos modelos.

---

## 🎯 Definição do Problema

O churn de clientes é um dos desafios mais críticos em empresas baseadas em assinatura, especialmente no setor de telecomunicações. Reter clientes existentes é significativamente mais barato do que adquirir novos.

Este projeto tem como objetivo desenvolver um modelo preditivo capaz de identificar clientes com alta probabilidade de churn, permitindo estratégias proativas de retenção e tomada de decisão orientada por dados.

---

## 📊 Dataset

- Dataset Telco Customer Churn
- Problema de classificação binária:
  - 0 → Cliente permanece
  - 1 → Cliente cancela (churn)

---

## ⚙️ Pipeline do Projeto

### 1. Processamento de Dados
- Remoção de variáveis irrelevantes (ex: customerID)
- Tratamento de variáveis categóricas com one-hot encoding
- Divisão treino/teste com estratificação

### 2. Modelos Base (Ensemble Learning)
- Regressão Logística
- Árvore de Decisão
- Random Forest
- Comparação de modelos usando acurácia e métricas de classificação

### 3. Gradiente Boosting (XGBoost)
- Implementação do classificador XGBoost
- Integração ao pipeline de pré-processamento
- Comparação de performance com modelos base

### 4. Aprendizado Semi-Supervisionado
- Simulação de dados não rotulados
- Self Training (pseudo rotulagem)
- Processo iterativo de propagação de rótulos
- Avaliação comparativa com modelos supervisionados

---

## 📈 Resumo de Resultados

O melhor modelo neste projeto foi:

- 🏆 Pipeline com XGBoost (~0.799 de acurácia)

O aprendizado semi-supervisionado (Self Training) apresentou desempenho competitivo, mas não superou o modelo supervisionado com XGBoost, destacando que sua eficácia depende fortemente da distribuição dos dados e da qualidade dos rótulos.

---

## 🧠 Principais Aprendizados

- Métodos de ensemble melhoram significativamente a performance base
- XGBoost é altamente eficaz para dados tabulares estruturados
- Aprendizado semi-supervisionado é poderoso, mas sensível à qualidade dos dados e suposições
- Um pipeline bem estruturado melhora a reprodutibilidade e escalabilidade

---

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## 📁 Estrutura do Repositório

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

## 🚀 Como Executar

git clone https://github.com/Vagnerkrg/advanced-classification-ml.git

cd advanced-classification-ml

python -m venv .venv

Windows:
.venv\Scripts\activate

Mac/Linux:
source .venv/bin/activate

pip install -r requirements.txt

---

## ▶️ Fluxo de Execução

Executar o notebook principal:

01_baseline_classification.ipynb

Este notebook contém o pipeline completo de machine learning:

- processamento de dados
- modelos base
- ensemble learning
- XGBoost pipeline
- aprendizado semi-supervisionado

---

## 📌 Próximos Passos

- Otimização de hiperparâmetros (GridSearch / RandomSearch)
- Análise de importância de variáveis
- Refinamento da abordagem semi-supervisionada
- Refatoração para estrutura modular em src/
- Melhoria da documentação com visualizações e insights

---

## 👨‍💻 Autor

Vagner Ferreira  
Cientista de Dados | Machine Learning | Engenharia de Dados  
Focado na construção de soluções de IA de ponta a ponta aplicadas a problemas reais