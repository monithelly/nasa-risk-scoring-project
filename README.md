# 🚀 Sistema de Priorização de Risco para Manutenção Preditiva (NASA CMAPSS)

## 📌 Visão Geral

Este projeto tem como objetivo identificar motores aeronáuticos com maior risco de falha, utilizando dados de sensores da NASA (CMAPSS). A solução combina análise exploratória, modelagem preditiva e uma camada de decisão baseada em score de risco, com foco em apoiar a priorização de manutenção.

---

## 🎯 Problema de Negócio

Falhas não previstas em motores aeronáuticos podem gerar:

- altos custos operacionais  
- riscos à segurança  
- paradas não planejadas  

Diante disso, surge a necessidade de responder:

> **Quais motores devem ser priorizados para manutenção preventiva?**

---

## 🧠 Abordagem

O projeto foi estruturado em três camadas principais:

### 1. Análise Exploratória
- Entendimento do comportamento temporal dos motores  
- Identificação de padrões de degradação ao longo dos ciclos  
- Avaliação inicial da relevância dos sensores  

### 2. Modelagem Preditiva
- Criação do RUL (Remaining Useful Life)  
- Transformação do problema em classificação de risco  
- Treinamento de modelo Random Forest  
- Avaliação com métricas de classificação (precision, recall, F1-score)  

### 3. Camada de Decisão
- Construção de um **Risk Score (0–100)** baseado na probabilidade de falha  
- Classificação dos motores em níveis de criticidade:  
  - 🔴 Alto risco  
  - 🟠 Médio risco  
  - 🟢 Baixo risco  
- Geração de ranking de priorização para manutenção  

---

## 📊 Principais Resultados

- F1-score de **0.83 para motores de alto risco**, indicando boa capacidade de identificar falhas críticas  
- Identificação dos sensores mais relevantes para o modelo:  
  - sensor_4  
  - sensor_11  
  - sensor_12  
  - sensor_7  

- Criação de um sistema de priorização que permite direcionar ações de manutenção de forma mais eficiente  

---

## 💡 Insights

- Sensores apresentam padrões consistentes de degradação ao longo do tempo  
- Classes extremas (alto e baixo risco) são bem separáveis pelo modelo  
- A classe intermediária apresenta maior ambiguidade, refletindo cenários reais de decisão  
- Nem todos os sensores contribuem igualmente — poucos concentram a maior parte do poder preditivo  

---

## 📊 Priorização de Motores por Risco

*(adicione aqui o gráfico depois)*

```markdown
![Top 10 Motores](reports/figures/top10_risk.png)

## 🛠️ Tecnologias

- Python
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn

---

## 📁 Estrutura do Projeto

- data/
- notebooks/
- src/
- reports/
 
---

## 🚀 🚀 Evoluções Futuras

- Implementação de interpretabilidade do modelo (SHAP) para explicar decisões de risco
- Desenvolvimento de interface interativa (Streamlit) para simulação de cenários
- Criação de dashboard executivo para acompanhamento de risco
- Integração com dados reais para validação em ambiente produtivo
- Evolução do modelo considerando comportamento temporal dos sensores

---

🧾 Conclusão

Este projeto demonstra como dados de sensores podem ser transformados em decisões operacionais, permitindo identificar motores críticos e priorizar ações de manutenção.

A abordagem integra análise de dados, modelagem preditiva e uma camada de decisão interpretável, aproximando o uso de machine learning de aplicações reais de negócio.

---

## 👩‍💻 Autora

Monithelly Simões  
Analista de Dados
