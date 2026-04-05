# 🌳 Previsão de Churn com Algoritmos Ensemble Baseados em Árvores

Aplicação completa do pipeline de Machine Learning (CRISP-DM) para prever churn de clientes, utilizando algoritmos ensemble baseados em árvores, com análise comparativa entre modelos e interpretação dos resultados.

---

## 📋 Descrição do Projeto

Este projeto aplica o pipeline CRISP-DM em um dataset do Kaggle sobre churn de clientes. O objetivo é identificar quais clientes têm maior probabilidade de cancelar o serviço, comparando o desempenho de quatro algoritmos ensemble baseados em árvores de decisão.

---

## 🗂️ Estrutura do Pipeline (CRISP-DM)

### 1. Entendimento de Negócio 
- Contextualização do problema de churn e objetivo do modelo
- Por que churn importa? Qual o impacto no negócio? O que será previsto?

### 2. Entendimento dos Dados 
- Exploração inicial com `head()`, `describe()`, `info()` e distribuição da variável target
- A base é balanceada? Quais variáveis são relevantes? Existem possíveis vieses?

### 3. Preparação dos Dados 
- Limpeza, remoção de colunas irrelevantes, encoding de variáveis categóricas e split treino/teste
- Justificativa para remoções e escolhas de encoding

### 4. Modelagem — Ensemble
Treinamento de **4 modelos**:
- 🌲 Random Forest
- ⚡ Gradient Boosting
- 🚀 XGBoost
- 💡 LightGBM

- Diferenças entre os modelos, complexidade e risco de overfitting

### 5. Avaliação Experimental 
- Métricas: `accuracy`, `precision`, `recall`, `F1-score` e `confusion matrix`
- O modelo acerta churn? O recall é adequado para o problema?

### 6. Análise Comparativa
- Comparação dos 4 modelos em tabela consolidada
- Qual é o melhor modelo? A diferença entre eles é relevante?

---

## 🛠️ Tecnologias Utilizadas

- Python 3.x
- Pandas / NumPy
- Scikit-learn
- XGBoost
- LightGBM
- Matplotlib / Seaborn
- Jupyter Notebook

---

## 📊 Dataset

Dataset de churn de clientes disponível no [Kaggle](https://www.kaggle.com/), contendo informações sobre comportamento, histórico e características dos clientes para previsão de cancelamento.

---

## ▶️ Como Executar

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/seu-repositorio.git

# Instale as dependências
pip install -r requirements.txt

# Abra o notebook
jupyter notebook
```

---

## 📈 Resultados

A análise comparativa entre os quatro modelos ensemble permite identificar o algoritmo com melhor equilíbrio entre **recall** (identificação correta de churners) e **precisão**, considerando o impacto de negócio de falsos negativos e falsos positivos.

---

## 📁 Estrutura de Arquivos

```
├── data/
│   └── churn_dataset.csv
├── notebook/
│   └── churn_pipeline.ipynb
├── requirements.txt
└── README.md
```
