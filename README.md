# Titanic Survival Prediction

Este projeto visa prever a sobrevivência de passageiros do Titanic usando um classificador de Random Forest. O objetivo é analisar dados de passageiros e aplicar técnicas de aprendizado de máquina para fazer previsões sobre a variável alvo `Survived`.

## Estrutura do Projeto

- **train.csv**: Conjunto de dados de treinamento contendo informações sobre passageiros.
- **test.csv**: Conjunto de dados de teste onde as previsões de sobrevivência serão realizadas.
- **submission.csv**: Arquivo gerado que contém as previsões de sobrevivência para cada passageiro do conjunto de teste.
- **correlacao.ipynb**: Código que mostra a correlação das variáveis em relação a `Survived`, além de filtrar o train.csv criando o train_f.csv.
- **test.ipynb**: Código que faz o pré-processamento do teste.csv e aplica o classificador.

## Descrição do Algoritmo

### Pré-processamento de Dados:

- Tratamento de dados nulos.
- Conversão de variáveis categóricas em numéricas (ex: Sex convertido em 1 e 2).
- Normalização da idade.

### Treinamento do Modelo:

- Utiliza RandomForestClassifier para treinar o modelo com o conjunto de dados de treinamento.
- Hiperparâmetros otimizados usando GridSearchCV.

### Predições:

Realiza previsões no conjunto de teste e salva os resultados no arquivo submission.csv.

### Avaliação do Modelo:

A matriz de confusão e a curva ROC/AUC são exibidas para avaliar o desempenho do modelo.

## Resultados

O modelo gerou um score público de ? no Kaggle, indicando a precisão das previsões de sobrevivência.