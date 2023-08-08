# Previsão do Tempo para a Cidade de Nova York
Este repositório contém um projeto de previsão do tempo para a cidade de Nova York, utilizando técnicas de machine learning, especificamente regressão linear e regressão Ridge. O objetivo é prever as condições climáticas com base nos dados históricos de 1970 a 2022.

## Etapas do Projeto
### 1. Coleta dos Dados
Os dados históricos de previsão do tempo para a cidade de Nova York foram coletados de fontes confiáveis, abrangendo o período de 1970 a 2022. Esses dados incluem informações como temperatura máxima, temperatura mínima, umidade, velocidade do vento e precipitação.

### 2. Limpeza dos Dados
Antes de prosseguir com a análise, os dados foram submetidos a um processo rigoroso de limpeza. Isso incluiu a remoção de valores ausentes, a correção de outliers e a normalização de dados, garantindo que o conjunto de dados estivesse pronto para ser utilizado no treinamento dos modelos de machine learning.

### 3. Preparação dos Dados para Machine Learning
Os dados foram divididos em conjunto de treinamento e conjunto de teste. Além disso, as características relevantes foram selecionadas e transformadas em formato adequado para alimentar os modelos de regressão. A normalização também foi aplicada para garantir que as características tivessem escalas comparáveis.

### 4. Treinamento dos Modelos
Foram utilizados dois modelos de regressão: regressão linear e regressão Ridge. A biblioteca scikit-learn (sklearn) foi empregada para implementar esses modelos. O conjunto de treinamento foi utilizado para treinar os modelos, permitindo que eles aprendessem os padrões presentes nos dados históricos.

### 5. Avaliação dos Modelos
Os modelos treinados foram avaliados usando o conjunto de teste. Foram utilizadas métricas como o erro médio absoluto (MAE) e o erro quadrático médio (MSE) para medir a eficácia das previsões. Comparar as métricas dos dois modelos permitiu determinar qual deles teve melhor desempenho na previsão do tempo.

## Tecnologias Utilizadas
- Python: A linguagem de programação principal para a implementação do projeto.
- Pandas: Utilizado para manipulação e análise dos dados.
- Scikit-learn (sklearn): Usado para criar e treinar os modelos de regressão.
- Jupyter Notebook: Utilizado para criar e executar o código de análise de dados de forma interativa.
