# Projetos-Alura
Uma empresa contratou você para analisar como o consumo de café influencia a qualidade do sono dos clientes.  Você terá acesso a um conjunto de dados com informações sobre idade, consumo de café, ingestão de cafeína, estresse, IMC, horas de sono e outros fatores.  Análise Exploratória de Dados (EDA) -> Visualização e Insights  ->  Modelo preditivo


# Health&Life Analytics — Café, Estresse e Sono

Projeto desenvolvido para analisar como o **consumo de café** e o **nível de estresse** influenciam a **qualidade do sono** dos clientes, utilizando **Análise Exploratória de Dados (EDA)**, **visualizações comparativas** e **modelos preditivos de Machine Learning**.

O objetivo final é apoiar **decisões de negócio** e **orientações de bem‑estar**, identificando perfis com maior risco de baixa qualidade de sono.

---

## 🎯 Objetivos do Projeto

- Realizar uma **análise exploratória completa (EDA)** do conjunto de dados
- Identificar padrões entre consumo de café, estresse e sono
- Criar **visualizações comparativas e segmentadas**
- Desenvolver modelos de **classificação** para prever `Sleep_Quality`
- Gerar **insights acionáveis** e **recomendações para o negócio**

---

## 📊 Conjunto de Dados

O dataset contém informações sintéticas de clientes com variáveis como:

- Idade
- Gênero
- Consumo de café (xícaras/dia)
- Ingestão de cafeína (mg/dia)
- Nível de estresse
- IMC (BMI)
- Atividade física
- Horas de sono
- Qualidade do sono (`Sleep_Quality`)

📄 Arquivo utilizado:
synthetic_coffee_health_10000(in).csv

## 🧪 Estrutura do Projeto

├── notebooks/
│   └── Projeto_Sono_HealthLife_v2.ipynb
├── data/
│   └── synthetic_coffee_health_10000(in).csv
├── outputs/
│   ├── dataset_processado.csv
│   └── best_sleep_quality_model.pkl
└── README.md

## 📈 Entrega #1 — Análise Exploratória (EDA)

- Avaliação da estrutura dos dados (shape, tipos, nulos e duplicados)
- Estatísticas descritivas para variáveis numéricas e categóricas
- Visualizações:
  - Histogramas e boxplots para variáveis numéricas
  - Gráficos de barras e pizza para variáveis categóricas
  - Matriz de correlação (heatmap)
- Comentários e interpretação dos principais padrões identificados

---

## 📊 Entrega #2 — Visualizações e Insights

- Gráficos comparativos entre **consumo de café** e **horas de sono**
- Segmentação por:
  - Nível de estresse
  - Gênero
  - Faixa etária × estresse
- Tipos de gráficos utilizados:
  - Dispersão com linha de tendência
  - Boxplots
  - Heatmaps
  - FacetGrid
- Seção dedicada a **Principais Descobertas**, com insights de negócio documentados

### 🔍 Principais Insights

- Clientes com **alto consumo de cafeína** dormem em média **~0,6 hora a menos**
- O **estresse** é o fator com maior impacto negativo no sono
- Diferenças por gênero são pouco relevantes
- Faixas etárias mais jovens apresentam maior sensibilidade à combinação **café + estresse**

---

## 🤖 Entrega #3 — Modelo Preditivo

### Pré-processamento
- Remoção de colunas irrelevantes
- Codificação de variáveis categóricas (One‑Hot Encoding)
- Padronização das variáveis numéricas
- Criação de **features derivadas**, como:
  - `Caffeine_per_Cup`
  - `Activity_per_BMI`

### Modelagem
- Divisão dos dados em **treino e teste (80/20, estratificado)**
- Modelos treinados:
  - Regressão Logística
  - Random Forest
- Avaliação com:
  - Acurácia
  - Matriz de confusão
  - Classification report (Precision, Recall, F1‑Score)

### Salvamentos
- Dataset final processado:
dataset_processado.csv

- Melhor modelo salvo:

best_sleep_quality_model.pkl

## 🧠 Recomendações para o Negócio

- Criar alertas para clientes com **alto consumo de cafeína e estresse elevado**
- Estimular a redução do consumo de café no período noturno
- Implementar programas de **gestão de estresse e higiene do sono**
- Utilizar o modelo preditivo para **segmentação de risco e campanhas personalizadas**

---

## ⚙️ Tecnologias Utilizadas

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit‑learn
- Jupyter Notebook

---

## ✅ Como Executar

1. Clone o repositório
2. Instale as dependências
3. Abra o notebook `Projeto_Sono_HealthLife_v2.ipynb`
4. Execute as células sequencialmente

---

## 📌 Observações Finais

Este projeto utiliza **dados sintéticos** e foi desenvolvido com foco educacional e analítico, seguindo boas práticas de ciência de dados, organização de código e clareza na comunicação de resultados.
