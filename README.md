# MVP - Machine Learning & Analytics

## Descrição do Problema

Neste projeto, utilizamos o conjunto de dados "Curva de Carga Horária" produzido e disponibilizado pelo Operador Nacional do Sistema Elétrico (ONS). O objetivo é treinar um modelo de machine learning para um problema de regressão, visando projetar, com base nos dados históricos, a carga de energia futura em base horária. Essa projeção é fundamental para o planejamento da operação e expansão do parque gerador de energia elétrica no Brasil, além de impactar outras aplicações, como o preço spot de energia elétrica.

## Fonte dos Dados

Os dados foram baixados do site do ONS. O dataset pode ser acessado em: [Curva de Carga Horária - ONS](https://dados.ons.org.br/dataset/curva-carga)

## Preparação dos Dados

1. **Carregamento dos Dados**: Os dados foram carregados e concatenados a partir de múltiplos arquivos CSV.
2. **Filtragem**: Foram utilizados apenas os dados do subsistema Sudeste/Centro-Oeste.
3. **Tratamento de Valores Nulos**: Linhas com valores nulos foram removidas.
4. **Feature Engineering**: Foram criadas features temporais para capturar padrões sazonais e tendências.

## Modelagem e Treinamento

Foram selecionados e treinados os seguintes modelos de machine learning e ensembles:

- **XGBoost (Extreme Gradient Boosting)**
- **LightGBM (Light Gradient Boosting Machine)**
- **Random Forest**
- **Linear Regression**
- **Voting Regressor Ensemble**
- **Stacking Ensemble**
- **Prophet**

## Resultados

- **Prophet** foi escolhido como o melhor modelo final, com os menores valores de erro em ambas as métricas avaliadas (RMSE e MAE).

## Conclusão

O objetivo do trabalho foi plenamente alcançado. O modelo Prophet mostrou-se o mais adequado para a projeção de carga de energia. Para futuras melhorias, sugere-se adicionar dados climáticos e econômicos que possam ajudar a explicar o comportamento da carga de energia.


