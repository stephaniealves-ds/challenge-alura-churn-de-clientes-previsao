# Projeto de Análise e Previsão de Evasão de Clientes (Churn) - Parte 2

Este repositório contém a segunda parte do projeto de análise e previsão de evasão de clientes (Churn) de uma empresa de telecomunicações fictícia.

A **Parte 1** do projeto focou na análise exploratória dos dados, limpeza, tratamento de valores ausentes e padronização inicial. O repositório correspondente pode ser encontrado em:

[🔗 Repositório da Parte 1](https://github.com/stephaniealves-ds/challenge-alura-churn-de-clientes)

## 🎯 Objetivo do Projeto

A segunda etapa do desafio tem como objetivo principal a construção de um pipeline de Machine Learning para prever a evasão de clientes. As principais fases do projeto incluíram:

1.  **Pré-processamento de Dados**: Continuação da preparação do dataset, transformando variáveis categóricas em numéricas e padronizando as colunas numéricas para uso em modelos preditivos.
2.  **Modelagem Preditiva**: Construção e treinamento de dois modelos de classificação (Regressão Logística e Random Forest).
3.  **Avaliação e Comparação**: Análise do desempenho dos modelos utilizando métricas robustas como Acurácia, Precisão, Recall e F1-Score, além da matriz de confusão.
4.  **Análise de Relevância**: Identificação das variáveis mais importantes para a previsão de evasão em cada modelo.
5.  **Relatório Final**: Elaboração de um relatório detalhado com os principais insights obtidos e propostas de estratégias de retenção de clientes.

## 🛠️ Tecnologias Utilizadas

* **Python**: Linguagem de programação principal.
* **Pandas**: Para manipulação e análise de dados.
* **NumPy**: Para suporte a operações numéricas.
* **Scikit-learn**: Para a construção e avaliação dos modelos de Machine Learning.
* **Matplotlib / Seaborn**: Para visualização de dados.

## 📁 Estrutura do Repositório

├── notebook_parte2.ipynb     # Notebook principal com o código e análises da parte 2

├── df_telecom_clean.csv      # Dataset limpo, resultante da parte 1

└── README.md                 # Este arquivo de documentação

## 📈 Principais Análises e Resultados

* **Melhor Modelo**: O modelo **Random Forest** apresentou o melhor desempenho geral, com um F1-Score superior, demonstrando maior capacidade de identificar corretamente os clientes que evadem (classe minoritária).

* **Fatores de Evasão**: A análise de importância das variáveis revelou que os fatores mais relevantes para a previsão de Churn são:
    * **Meses de Contrato (`Meses_de_Contrato`)**: A baixa permanência é o principal fator de risco.
    * **Serviço de Internet_Fiber optic**: Usuários de fibra óptica apresentam um risco elevado de Churn.
    * **Tipo de Contrato_Month-to-month**: Contratos com pouca fidelidade são um forte indicador de evasão.
    * **Cobranca_Mensal**: O aumento da cobrança mensal está diretamente associado a uma maior propensão à evasão.
