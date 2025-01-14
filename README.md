# Detecção de Fraudes em Cartões de Crédito

## Visão Geral

Este projeto aplica técnicas de **Machine Learning** para detectar transações fraudulentas em cartões de crédito, utilizando um dataset altamente desbalanceado. A solução foi construída com **Python**, **Jupyter Notebook** e **XGBoost** para identificar fraudes com alta precisão.

## Tecnologias Usadas

- **Python & Jupyter Notebook**: Ferramentas principais para análise de dados e implementação de modelos de machine learning.
- **XGBoost**: Algoritmo de **Gradient Boosting** com desempenho excepcional (AUC-ROC de 0.9704) para detectar fraudes em cenários desbalanceados.
- **Random Forest**: Alternativa robusta e interpretável, mas com desempenho inferior ao XGBoost (AUC-ROC de 0.9068).
- **SMOTE**: Técnica de **oversampling** para balancear as classes no dataset e melhorar a performance do modelo.

## Resultados

- **Melhor Modelo**: **XGBoost**, com AUC-ROC de **0.9704**, demonstrando alta precisão e eficiência.
- **Random Forest**: AUC-ROC de **0.9068**, ainda bom, mas menos eficiente comparado ao XGBoost.
- **Feature Importance**: Variáveis como `V14`, `V12`, e `V4` foram cruciais para a detecção das fraudes, enquanto `Amount` e `Time` tiveram menor impacto.

## Como Funciona

1. **Análise Exploratória**: Identificação do desbalanceamento das classes.
2. **Pré-processamento**: Aplicação do SMOTE para balancear as classes.
3. **Treinamento**: Teste de múltiplos algoritmos, com foco em **XGBoost**.
4. **Avaliação**: AUC-ROC para medir o desempenho em cenários desbalanceados.

## Contato

- **Autor**: Hian Stafford
- **Email**: hian.correa@gmail.com
