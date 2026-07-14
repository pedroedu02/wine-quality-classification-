# 🍷 Wine Quality Classification using Machine Learning

## Tech Challenge 2 - Pós Tech Data Analytics

Este projeto foi desenvolvido como parte do **Tech Challenge 2** da Pós-Graduação **Pós Tech em Data Analytics**, tendo como objetivo aplicar técnicas de **Machine Learning** para prever a qualidade de vinhos a partir de suas características físico-químicas.

---

## 👨‍🎓 Autor

**Pedro Garcia**  
**RM:** 374179

---

## 📖 Sobre o Projeto

A avaliação da qualidade de um vinho é tradicionalmente realizada por especialistas, considerando fatores como aroma, sabor e equilíbrio. Entretanto, esse processo pode ser subjetivo e depender da experiência do avaliador.

Neste projeto foi desenvolvido um modelo de classificação capaz de prever se um vinho possui **Alta Qualidade** ou **Baixa/Média Qualidade**, utilizando apenas informações físico-químicas obtidas durante sua produção.

A base de dados utilizada foi o **WineQT Dataset**, contendo variáveis como:

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol

A variável **quality** foi transformada em uma classificação binária:

- **Alta Qualidade:** Quality ≥ 7
- **Baixa/Média Qualidade:** Quality < 7

---

## 🎯 Objetivo

Desenvolver uma pipeline completa de Machine Learning capaz de classificar a qualidade dos vinhos utilizando suas características físico-químicas, aplicando os conceitos estudados durante a disciplina.

---

## 🔍 Etapas Desenvolvidas

O projeto foi dividido nas seguintes etapas:

- Compreensão do problema;
- Importação e análise inicial da base de dados;
- Limpeza e validação dos dados;
- Análise Exploratória dos Dados (EDA);
- Distribuição das variáveis;
- Identificação de correlações;
- Detecção de outliers;
- Análise do balanceamento das classes;
- Pré-processamento dos dados;
- Padronização das variáveis utilizando StandardScaler e MInMaxScaler;
- Separação entre dados de treino e teste;
- Treinamento dos modelos de Machine Learning;
- Validação Cruzada (Cross Validation);
- Otimização de hiperparâmetros utilizando **GridSearchCV**;
- Avaliação e comparação dos modelos;
- Interpretação dos resultados obtidos.

---

## Modelos Utilizados

Durante o desenvolvimento foram treinados e avaliados os seguintes modelos:

- Regressão Logística
- K-Nearest Neighbors (KNN)
- KNN Otimizado utilizando GridSearchCV

Os modelos foram avaliados utilizando as métricas:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC AUC
- Classification Report
- Matriz de Confusão
- Curva ROC

---

## 📊 Principais Resultados

Os modelos apresentaram desempenho satisfatório na classificação da qualidade dos vinhos.

Após a comparação entre os algoritmos, o **KNN Otimizado** apresentou o melhor desempenho geral, alcançando aproximadamente:

| Métrica | Resultado |
|----------|-----------:|
| Accuracy | **88,21%** |
| Precision | **63,16%** |
| Recall | **37,50%** |
| F1-Score | **47,06%** |
| ROC AUC | **79,82%** |

Embora a Regressão Logística tenha apresentado a maior ROC AUC e o KNN padrão tenha obtido melhor Recall, o **KNN Otimizado** foi escolhido como modelo final por apresentar maior acurácia e maior precisão, reduzindo significativamente a quantidade de classificações incorretas de vinhos comuns como sendo de alta qualidade.

---

## 📌 Conclusão

O projeto mostrou que, mesmo utilizando modelos relativamente simples, é possível obter um bom desempenho na classificação, contribuindo para auxiliar especialistas na tomada de decisão e no controle da qualidade durante o processo produtivo.

---

## 🛠️ Tecnologias Utilizadas

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-Learn

---

## 📂 Estrutura do Projeto

```text
wine-quality-classification/
│
├── data/              # Base de dados utilizada
├── notebooks/         # Notebook com toda a análise e modelagem
├── src/               # Scripts auxiliares
├── results/           # Gráficos e resultados obtidos
├── requirements.txt   # Bibliotecas utilizadas
└── README.md          # Documentação do projeto
```

---

## 📚 Base de Dados

**WineQT Dataset**

Dataset público utilizado para fins acadêmicos contendo informações físico-químicas de diferentes amostras de vinho e suas respectivas avaliações de qualidade.

---

**Projeto desenvolvido para o Tech Challenge 2 da Pós Tech em Data Analytics.**
