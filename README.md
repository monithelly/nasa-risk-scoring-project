# 🚀 Sistema de Priorização de Risco para Manutenção Preditiva (NASA CMAPSS)

## 📌 Visão Geral

Este projeto tem como objetivo identificar motores aeronáuticos com maior risco de falha, utilizando dados de sensores da NASA (CMAPSS), combinando análise exploratória, modelagem preditiva e uma camada de decisão baseada em score de risco.

---

## 🎯 Problema de Negócio

Falhas não previstas em motores podem gerar:

- altos custos operacionais
- riscos de segurança
- paradas não planejadas

Diante disso, surge a necessidade de responder:

> **Quais motores devem ser priorizados para manutenção?**

---

## 🧠 Abordagem

O projeto foi estruturado em três camadas principais:

### 1. Análise Exploratória
- Entendimento do comportamento temporal dos motores
- Identificação de padrões de degradação
- Avaliação de sensores relevantes

### 2. Modelagem Preditiva
- Criação do RUL (Remaining Useful Life)
- Transformação em categorias de risco
- Treinamento de modelo Random Forest
- Avaliação com métricas de classificação

### 3. Camada de Decisão
- Criação de um **Risk Score (0–100)**
- Classificação dos motores em:
  - 🔴 Alto risco
  - 🟠 Médio risco
  - 🟢 Baixo risco

---

## 📊 Principais Resultados

- F1-score de **0.82 para motores de alto risco**
- Identificação dos sensores mais relevantes:
  - sensor_4
  - sensor_11
  - sensor_12
  - sensor_7

- Criação de um sistema interpretável para priorização de manutenção

---

## 💡 Insights

- Sensores apresentam padrões claros de degradação ao longo do tempo
- Classes extremas (alto e baixo risco) são bem separáveis
- Classe intermediária apresenta maior ambiguidade, refletindo cenários reais

---

## 🛠️ Tecnologias

- Python
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn

---

## 📁 Estrutura do Projeto
<img width="1170" height="752" alt="image" src="https://github.com/user-attachments/assets/8dc79427-1985-4dd8-bec0-c1ae5f395f55" />

- data/
- notebooks/
- src/
- reports/
 
---

## 🚀 Próximos Passos

- Refinar feature engineering
- Implementar interpretabilidade (SHAP)
- Criar dashboard ou aplicação interativa (Streamlit)
- Evoluir para modelo mais robusto

---

## 👩‍💻 Autora

Monithelly Simões  
Analista de Dados
