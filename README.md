# 🧠 Previsão de Valor Total de Pedidos Mensais com Machine Learning

Este projeto utiliza aprendizado de máquina para prever o **valor total de pedidos por empresa** no mês de **abril de 2025**, com base em dados históricos de compras mensais e características associadas a usuários, empresas, produtos e preços.

## 📊 Objetivo

Antecipar o valor total de pedidos feitos por empresas com um mês de antecedência, usando um modelo de regressão. Isso pode auxiliar na tomada de decisões comerciais, como controle de estoque, gestão de fornecedores e projeções de receita.

## ⚙️ Tecnologias Utilizadas

- **Python** (pandas, numpy, scikit-learn)
- **HistGradientBoostingRegressor** como modelo preditivo
- **Jupyter Notebook / VSCode** para desenvolvimento
- **Feature Engineering** com lags, diffs e one-hot encoding

## 🧩 Etapas do Projeto

1. **Carregamento e Conversão de Datas**  
   Conversão de colunas de data para o tipo `datetime`.

2. **Merge de múltiplos DataFrames**  
   Unificação dos dados de pedidos, produtos, usuários, empresas, preços, descontos, etc.

3. **Engenharia de Atributos**
   - Cálculo de demanda mensal
   - Criação de variáveis de defasagem (lag)
   - Extração de diferenças (diffs)
   - Codificação de mês e tipos de empresa (one-hot encoding)

4. **Separação Treino/Teste**
   - Treino: Dados até março/2025
   - Teste: Abril/2025

5. **Treinamento e Avaliação**
   - Escalonamento dos dados com `StandardScaler`
   - Modelo treinado com `HistGradientBoostingRegressor`
   - Métrica de avaliação: RMSE (Root Mean Squared Error)

6. **Previsões**
   - Geração de previsões e comparação com valores reais

## 📈 Resultado Final

📌 Projeto desenvolvido com a colaboração do Professor da Unichristus: **Pedro Bandeira** na etapa de imersão do Programa Residência em TIC-20 - Capacita Brasil/C-Jovem como parte de portfólio em Ciência de Dados com foco em previsão temporal de valores baseada em dados históricos de compras mensais e características associadas.
